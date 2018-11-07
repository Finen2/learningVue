<template>
  <div class="rootEmement">

    <div class="Main">
      <div class="partMain">
        Väder
      </div>
      <div class="partMain">
        Meddelanden
      </div>
      <div class="partMain">
        Kalender
      </div>
    </div>

    <div class="Main Clock">
      <h3>TS Counter</h3>
      <div>{{count}} is {{isOdd}}</div>
      <div>
      <button @click="increment()">INCREMENT</button>
      </div>
    </div>
  </div>

</template>

<script lang?"ts">
  import * as Vue from 'vue'
  import Component from 'vue-class-component'

  @Component
  export default class Counter extends Vue {
    count = 0
    increment() { this.count++ }
    get isOdd() {
      return (this.count%2 === 0) ? 'even' : 'odd'
    }
  }
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.rootEmement{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}

  .Main {
    background-color: #F6FFFF;
    height: calc(100vh - 4em);
    width: 80vw;
    margin-top: 4em;

    display: flex;
    flex-direction: row;
    flex-wrap: wrap;

    .partMain{
      background-color: #00A6C4;
      height: 70vh;
      width: 20vw;
      margin-top: 12.5vh;
      margin-left: 5vw;
      border-radius: 3em;
      color: white;
    }
  }
  .Clock{
    background-color: green;
    width: 20vw;
    padding-top: 100px;
  }


  section.section {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 140px;
    background: transparent;
  }

  h3.is-3, p.time {
    color: white;
  }

  h3.is-3:not(:last-child) {
    margin: 0;
    padding: 0;
  }

  .time {
    font-size: 7em;
  }
</style>
