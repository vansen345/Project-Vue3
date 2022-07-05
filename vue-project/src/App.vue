<script lang="ts">
import { defineComponent } from "vue";
import { ElContainer, ElHeader, ElMain } from "element-plus";
import Navbar from "./components/NavBar/Navbar.vue";
import Profile from "./components/Profile/Profile.vue";

export default defineComponent({
  components: {
    ElContainer,
    ElHeader,
    ElMain,
    Navbar,
    Profile,
  },
});
</script>

<template>
  <el-container class="container">
    <el-header style="background: aliceblue">
      <navbar />
    </el-header>
    <div class="body">
      <profile/>

    </div>

  </el-container>
</template>

<style>
@import "@/assets/base.css";
.container {
  width: 100%;
}
.body {
  width: 100%;
  height: 100%;
}
#app {
  width: 100%;
  font-weight: normal;
}
</style>
