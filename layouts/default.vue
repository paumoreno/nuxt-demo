<template>
  <div class="App">
    <nav class="App__nav">
      <nuxt-link class="App__navLink" :to="{name:'index'}">Hello world</nuxt-link>
      <nuxt-link class="App__navLink" :to="{name:'planets'}">Hello planets</nuxt-link>
    </nav>
    <div class="App__payload">
      <nuxt/>
    </div>
  </div>
</template>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}

.App {
  width: 100vw;
  height: 100vh;
}

.App__nav {
  display: flex;
  align-items: center;
  justify-content: space-around;
  height: 3em;
  background-color: #222;
}

.App__navLink {
  display: inline-block;
  text-decoration: none;
  color: white;
  padding: .5em .8em;
  border-radius: 10em;
}

.nuxt-link-exact-active {
  background-color: white;
  color: #222;
}

.App__payload {
  height: calc(100vh - 3em);
  background-color: black;
}
</style>

