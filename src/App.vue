<template id="app">
  <router-view/>
</template>

<style>
  :root {
    --fontPrimary: 'Fjalla One', sans-serif;;
    --fontSecondary: 'Open Sans', sans-serif;
  }

  * {
    margin: 0;
    padding: 0;
  }

  html {
    scroll-behavior: smooth;
  }

  body {
    background: #121212;
  }

  a {
    text-decoration: none;
    cursor: pointer;
  }

  button {
    background: none;
    border: none;
    cursor: pointer;
  }

  li {
    list-style-type: none;
  }

  .separator-hr {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 2rem 0;
  }

  .separator-hr > hr {
    width: 90%;
    border: solid 1px #B64FC8;
  }

</style>