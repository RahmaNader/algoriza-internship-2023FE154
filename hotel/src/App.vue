<template>
  <div class="navbar">
    <div class="navbar-left">
      <img src="@/assets/logonavbar.png" alt="Description of Image">
      <p>my Dream place</p>
    </div>
    <div class="navbar-middle">
      <ul class="navbar-items">
        <li><router-link to="/" class="navbar-item">Home</router-link></li>
        <li class="navbar-item">Discover</li>
        <li class="navbar-item">Activities</li>
        <li><router-link to="/about" class="navbar-item">About</router-link></li>
        <li class="navbar-item">Contact</li>
      </ul>
    </div>
    <div class="navbar-right">
      <router-link to="/login" class="button-link">Login</router-link>

    </div>
  </div>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 0 20px 0 20px;
}

.navbar-left {
  margin-right: auto;
  display: flex;
  align-items: center;
}

.navbar-middle {
  flex-grow: 1;
  margin: 0 180px;
}

.navbar-items {
  display: flex;
  justify-content: space-between;
  list-style: none;
  padding: 0;
}

.navbar-item {
  margin-right: 10px;
  text-decoration: none;
  color: black;
}

.navbar-right {
  margin-left: auto;
}
.navbar-button, .button-link {
    width: 82px;
    height: 43px;
    background: #2F80ED;
    border-radius: 6px;
    border: none;
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 20px;
    letter-spacing: 0.02em;
    color: #FFFFFF;
    cursor: pointer;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center; 
    text-decoration: none;
}

li,p {
    color: #333333;
    font-style: normal;
    cursor: pointer;
}
router-link {
  text-decoration: none;
}

</style>
