<template>
  <div class="App">
    <header class="App-header">
      <img src="../assets/logo.png">
      <h1 class="App-title">Hello Wormhole</h1>
    </header>
    <div class='App-content'>
    </div>
  </div>
</template>

<script>
let Wormhole = require('wormholecash/lib/Wormhole').default
let wormhole = new Wormhole()

export default {
  name: 'BitBox'
}
</script>

<style scoped>
  .App {
    font-family: sans-serif;
    max-width: 100%;
    word-wrap: break-word;
  }
</style>
