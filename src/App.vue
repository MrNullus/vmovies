<template>
  <header>
    <router-link to="/">
      <h1><span>V</span>Movies</h1>
    </router-link>
  </header>
   <div style="height: 2px; background-image: linear-gradient(to right, rgb(0 255 126), rgb(0, 255, 255));"></div>
  <main>
    <router-view/>
  </main>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Fascinate+Inline&family=Roboto+Slab:wght@100..900&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Roboto Slab", serif;
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
  color: #f1f1c1;
  letter-spacing: 1pt;

  &::selection {
    background: transparentize(#42B883, 0.5);
  }
}

h1 {
  font-family: "Fascinate Inline", system-ui;
  font-weight: 400;
  font-style: normal;
}

body {
  background-color: #000000eb;
}

a {
  text-decoration: none;
}

header {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px 16px;
  background-color: #101e1c;
  box-shadow: 0px 0px 4px rgb(32 255 146 / 26%);
  margin-bottom: 4px;

  h1 {
    color: #FFF;
    font-size: 3rem;

    span {
      color: #42B883;
      font-family: "Fascinate Inline", system-ui;
      font-weight: 400;
      font-style: normal;
    }
  }
}
</style>
