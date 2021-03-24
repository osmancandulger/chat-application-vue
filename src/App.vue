<template>
  <div id="app">
    <link
      href="https://fonts.googleapis.com/css2?family=Mulish:wght@200;400;500;700&display=swap"
      rel="stylesheet"
    />
    <link
      href="https://fonts.googleapis.com/icon?family=Material+Icons"
      rel="stylesheet"
    />
    <div class="container">
      <Sidebar />
    </div>
  </div>
</template>

<script>
import Sidebar from "@/components/Sidebar.vue";
export default {
  name: "App",
  components: { Sidebar },
};
</script>

<style lang="scss">
#app {
  font-family: "Mulish", Avenir, Helvetica, Arial, sans-serif;
  color: #2c3e50;
}
body {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100vh;
  background: #dcdfe6;
}
.container {
  display: flex;
  width: 1080px;
  height: 677px;
  border-radius: 20px;
  background: #fff;
}
</style>
