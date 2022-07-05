<script lang="ts">
import { defineComponent } from "vue";
import { ElContainer, ElHeader, ElMain } from "element-plus";
import Navbar from "./components/NavBar/Navbar.vue";

export default defineComponent({
  components: {
    ElContainer,
    ElHeader,
    ElMain,
    Navbar,
  },
});
</script>

<template>
  <el-container class="container">
    <el-header style="background: aliceblue">
      <navbar />
    </el-header>
    <el-main>Main</el-main>
  </el-container>
</template>

<style>
@import "@/assets/base.css";
.container {
  width: 100%;
}
#app {
  width: 100%;
  font-weight: normal;
}
</style>
