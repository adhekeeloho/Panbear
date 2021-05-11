<template id="app">
  <div id="nav">
    <nav class="navbar navbar-expand-lg navbar-dark red ml-auto fixed-top">
      <div class="d-flex bd-highlight mt-2">
        <img
          class="mr-auto img-fluid rounded-circle"
          style="width: 4rem; margin-bottom: 5px"
          src="./assets/logo.png"
        />
        <h5
          class="text-white font-weight-bolder"
          style="
            margin-left: 10px;
            margin-top: 18px;
            font-family: 'Poppins', sans-serif;
          "
          data-toggle="collapse"
          data-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          Panbear
        </h5>
      </div>
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item active">
            <router-link
              to="/"
              class="let text-light d-flex"
              style="font-family: 'Poppins', sans-serif"
              >Home</router-link
            >
          </li>
          <li class="nav-item active">
            <router-link
              to="/about"
              class="let text-light d-flex"
              style="font-family: 'Poppins', sans-serif"
              >About</router-link
            >
          </li>
          <li class="nav-item active">
            <router-link
              to="/Services"
              class="let text-light d-flex"
              style="font-family: 'Poppins', sans-serif"
              >Services</router-link
            >
          </li>
          <li class="nav-item active">
            <router-link
              to="/Contact"
              class="let text-light d-flex"
              style="font-family: 'Poppins', sans-serif"
              >Contact</router-link
            >
          </li>
        </ul>
      </div>
    </nav>
  </div>
  <router-view />
</template>

<script></script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding-top: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.red {
  background-color: rgb(29, 126, 159);
  overflow: hidden;
  text-align: center;
  text-decoration: none;
}

.let {
  padding-top: 14px 30px;
  margin-right: 30px;
  font-size: 17px;
}
</style>
