<template>
  <div>
    <!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/dashboard">Dashboard</router-link> -->
  </div>
  <router-view/>
</template>

<style>
body { 
  font-family: 'Poppins', sans-serif;
  background-color: #163e52;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

::root {
  --sidebar-bck: #244D61;
}
</style>
