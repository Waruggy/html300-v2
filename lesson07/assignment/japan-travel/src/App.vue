<template>
  <div class="main">
    <div class="container">
      <!-- Header -->
      <div class="row header">
          <h1>Japan Travel</h1>
      </div>
      <!-- Navbar with routes to other pages -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="navbar">
          <ul class="navbar-nav mr-auto mt-2 mt-lg-0">
              <li class="nav-item">
                <router-link class="nav-link" to="/">Home</router-link>
              </li>
                <li class="nav-item">
              <router-link class="nav-link" to="/Blog">Blog</router-link>
              </li>
              <li class="nav-item">
                <router-link class="nav-link" to="/Prefectures">Prefectures</router-link>
              </li>
              <li class="nav-item">
                <router-link class="nav-link" to="/About">About</router-link>
              </li>
            </ul>
          </div>
      </nav>
    <router-view/>
  </div>
</div>
</template>

<style lang="scss">
// Store page content
@import "../scss/_base.normalize.scss";
@import "../scss/_components.content.scss";
@import "../scss/_settings.responsive.scss";
@import "../scss/_settings.variables.scss";
@import "../scss/style.scss";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #fcc9b9;
}
// Format nav bar
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #fcc9b9;
    &.router-link-exact-active {
      color: red;
    }
  }
}

// Format header
.header {
  display: flex;
  font-family: 'Roboto Condensed', sans-serif;
  font-size: 60px;
  justify-content: center;
  align-items: center;
}

</style>
