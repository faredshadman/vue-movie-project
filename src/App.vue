<template>
  <header>
    <router-link to="/">
      <h1><span> Vue </span> Movies Header</h1>
    </router-link>
  </header>
  <main>
    <router-view />
  </main>
  <footer>
    <router-link to="/">
      <h1><span> Vue </span> Movies Footer</h1>
    </router-link>
  </footer>
</template>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Fira Sans", sans-serif;
  &::selection {
    background: transparentize($color: #42b883, $amount: 0.5);
  }
}
main {
  min-height: 90vh;
}
body {
  background: #35495e;
}
a {
  text-decoration: none;
}
header,
footer {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px 16px;
  background: #2c3d4e;
  box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.2);
  h1 {
    color: #fff;
    font-size: 28px;
    span {
      color: #42b883;
    }
  }
}
</style>
