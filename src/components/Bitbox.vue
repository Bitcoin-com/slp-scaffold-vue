<template>
  <div class="App">
    <header class="App-header">
      <img src="../assets/logo.png" />
      <h1 class="App-title">Hello Wormhole</h1>
    </header>
    <div class="App-content"></div>
  </div>
</template>

<script>
let SLPSDK = require("slp-sdk");
let SLP = new SLPSDK()(async () => {
  try {
    let list = await SLP.list();
    console.log(list);
  } catch (error) {
    console.error(error);
  }
})();

export default {
  name: "BitBox"
};
</script>

<style scoped>
.App {
  font-family: sans-serif;
  max-width: 100%;
  word-wrap: break-word;
}
</style>
