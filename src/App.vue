<template>
<!-- 新增 navbar -->
<nav class="navbar navbar-expand-lg navbar-light bg-light mb-4">
  <div class="container-fluid">
    <a class="navbar-brand fs-3 mx-3" href="#">Vue 3</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item mx-3">
          <router-link to="/" class="nav-link">Home</router-link>
        </li>
        <li class="nav-item mx-3">
          <router-link to="/about" class="nav-link">About</router-link>
        </li>
        <li class="nav-item mx-3">
          <router-link to="/newpage" class="nav-link">NewPage</router-link>
        </li>
      </ul>
    </div>
  </div>
</nav>
<div class="container" style="height: 300vh">
  <router-view></router-view>
</div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
