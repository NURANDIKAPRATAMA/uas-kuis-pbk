<template>
  <div id="app">
    <header class="header">
      <nav class="navbar">
        <ul class="nav-list">
          <li class="nav-item"><router-link to="/">Weather</router-link></li>
          <li class="nav-item"><router-link to="/location">Location</router-link></li>
          <li class="nav-item"><router-link to="/stopwatch">Stopwatch</router-link></li>
          <li class="nav-item"><router-link to="/tictactoe">Tic Tac Toe</router-link></li>
          <li class="nav-item"><router-link to="/photo">Photo</router-link></li>
        </ul>
      </nav>
    </header>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
#app {
  text-align: center;
}

.header {
  background: linear-gradient(to right, #ff6f00, #ffa000);
  padding: 20px;
  color: #fff;
}

.navbar {
  display: flex;
  justify-content: center;
  align-items: center;
}

.nav-list {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
}

.nav-item {
  margin-right: 10px;
}

.nav-item a {
  color: #fff;
  text-decoration: none;
  padding: 5px 10px;
  border-radius: 5px;
  transition: background-color 0.3s ease;
}
body {
  background-image: url(https://wallpaperaccess.com/full/731631.jpg);
}
.nav-item a:hover {
  background-color: #fff;
  color: #ff6f00;
}

.router-link-active a {
  background-color: #fff;
  color: #ff6f00;
}
</style>
