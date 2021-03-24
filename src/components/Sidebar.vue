<template>
  <div id="sidebar">
    <div class="logo">
      <span class="material-icons"> details </span>
    </div>
    <nav>
      <ul>
        <!-- 71x260 -->
        <li>
          <a href="#"><span class="material-icons"> speed </span></a>
        </li>
        <li>
          <a href="#"><span class="material-icons"> add_task </span></a>
        </li>
        <li>
          <a href="#"><span class="material-icons"> visibility </span> </a>
        </li>
        <li>
          <a href="#"><span class="material-icons"> people </span></a>
        </li>
        <li>
          <a href="#"><span class="material-icons"> insert_chart </span></a>
        </li>
        <li>
          <a href="#"><span class="material-icons"> videocam </span></a>
        </li>
      </ul>
    </nav>
    <div class="footer-profile">
      <span class="material-icons"> account_circle </span>
    </div>
  </div>
</template>

<script>
export default {
  el: "Sidebar",
  name: "Sidebar",
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
#sidebar {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  width: 71px;
  height: 100%;
  position: relative;
  border-right: 2px solid red;
  padding: 25px 0;
}
nav {
  display: flex;
  justify-content: center;
  width: 100%;
  height: 315px;
}
.logo {
  transform: rotate(-45deg);
  cursor: pointer;
  transition: all 0.4s ease;
  &:hover {
    transform: rotate(-45deg) scale(1.25);
  }
}
ul {
  display: flex;
  position: relative;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  list-style-type: none;
}
li {
  display: flex;
  position: relative;
  align-items: center;
  justify-content: center;
  width: 43px;
  height: 43px;

  border-radius: 10px;
  span {
    opacity: 0.65;
  }

  & + li {
  }
  &:hover {
    background: #e0f4f1;
  }
}
a {
  color: #2c3e50;
  text-decoration: none;
}
.footer-profile {
  cursor: pointer;
}
</style>
