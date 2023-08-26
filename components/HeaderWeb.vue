<template>
  <header class="header-wrapper">
    <div class="container">
      <h1><a href="#">ROTAMA Service</a></h1>
      <ul>
        <li>
          <n-link to="/">Home</n-link>
        </li>
        <li>
          <n-link to="/pages/profile.vue">Our Profile</n-link>
        </li>
        <li>
          <n-link to="/">Service</n-link>
        </li>
        <li>
          <n-link to="/">Message Us</n-link>
        </li>
      </ul>
    </div>
  </header>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
}
body {
  background-color: hsla(169, 44%, 78%, 0.5);
}
header {
  background-color: lightslategray;
}

.container {
  width: 80%;
  margin: auto;
}

.container:after {
  content: '';
  display: block;
  clear: both;
}

header h1 {
  float: left;
  padding: 5px 0;
}
header {
  background-color: lightslategray;
}

.container {
  width: 80%;
  margin: auto;
}

.container:after {
  content: '';
  display: block;
  clear: both;
}

header h1 {
  float: left;
  padding: 5px 0;
}

header h1 a {
  text-decoration: none;
  color: #1bec3e;
}

header ul {
  float: right;
}

header ul li {
  display: inline-block;
}

header ul li a {
  display: inline-block;
  padding: 14px;
  text-decoration: none;
  color: #fff;
}

header ul li a:hover {
  color: #fff;
  background-color: #148f77;
}
</style>
