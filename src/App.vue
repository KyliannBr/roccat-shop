<template>
  <div id="nav">
    <div class="logo">
      <img src="../src/assets/img/roccat-logo.png" alt="Logo">
    </div>
    <router-link to="/">Accueil</router-link> |
    <router-link to="/Mouses">Souris gaming</router-link>
  </div>
  <router-view/>
</template>

<style>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

:root {
  --res: calc(0.01 * 10vmin);
  --medium-slate-blue: #7765e3ff;
  --rich-black: #093a3eff;
  --bittersweet: #ff6666ff;
  --bluetiful: #3b60e4ff;
  --white: #ffffff;
  --mint-green: #b2ffa9;
}

::-webkit-scrollbar {
  width: 0;
}

  

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--white);
  background-color: var(--white);
}

#nav {
  height: 7vh;
  display: flex;
  place-items: center;
  background-color: #1a1a2b;
  padding: 0 2rem;
}

.logo {
  margin: 0 2rem;
}

.logo img{
  width: 50px;
}

#nav a {
  font-weight: bold;
  color: var(--white);
  padding: 2rem;
  font-size: calc(20 * var(--res));
  text-decoration: none;
  position: relative;
  transition: all .3s;
}

#nav a:hover {
  transition: all .3s;
  transform: translateY(-5px);
  color: var(--medium-slate-blue);
}

#nav a.router-link-exact-active {
  transform: translateY(-5px);
  color: #b2ffa9;
}
</style>
