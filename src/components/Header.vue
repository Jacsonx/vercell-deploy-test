<template>
  <div>
    <header class="header">
      <div id="nav">
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
      </div>
    </header>
    <router-view />
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {
    msg: String,
  },
};
</script>
<style  scoped>
@import url("https://fonts.googleapis.com/css2?family=Hind&display=swap");

.header {
  width: "100%";
  left: 0px;
  top: 0px;
  height: 90px;
  right: 0px;
  position: absolute;
  background-color: #1c1c1cf0;
}

#nav {
  font-family: "Hind", sans-serif;
  position: absolute;
  top: 30px;
  right: 0px;
}

#nav a {
  border-radius: 25%;
  border: 0px solid;
  color: bisque;
  margin: 20px;
  text-decoration: none;
  padding: 20px;
}

#nav a:hover {
  transition: 1s;
  background-color: bisque;
  color: black;
}
</style>
