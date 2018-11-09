<template>
  <div class="rootEmement">

    <div class="Main">
      hjfsak
    </div>

    <div class="Main Clock">
      hfjak
    </div>
  </div>

</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.rootEmement{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}

  .Main {
    background-color: black;
    height: calc(100vh - 4vh);
    width: 80vw;
    margin-top: 4vh;
  }
  .Clock{
    background-color: pink;
    width: 20vw;
  }
</style>
