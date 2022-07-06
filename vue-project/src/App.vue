<script lang="ts">
import { defineComponent } from "vue";
import { ElContainer, ElHeader, ElMain } from "element-plus";
import Navbar from "./components/NavBar/Navbar.vue";
import Profile from "./components/Profile/Profile.vue";
import Story from "./components/Story/storyComponent.vue";

export default defineComponent({
  components: {
    ElContainer,
    ElHeader,
    ElMain,
    Navbar,
    Profile,
    Story,
  },
});
</script>

<template>
  <el-container class="container">
    <el-header class="header">
      <navbar />
    </el-header>
    <div class="body">
      <div class="body-container">
        <div class="body-profile">
          <profile />
        </div>
        <div class="body-news">
          <story />
        </div>
      </div>
    </div>
  </el-container>
</template>

<style>
@import "@/assets/base.css";
.container {
  width: 100%;
}
.header {
  background: white;
  display: flex;
}
.body {
  width: 100%;
  height: 100%;
  
}
.body-container {
  width: 100%;
  display: flex;
}
.body-news {
  width: 50%;
  margin-top: 2rem;
}
.body-profile {
  width: 259px;
  margin-left: 5rem;
  flex: 0 0 259px;
  margin-top: 1.6rem;
}
#app {
  width: 100%;
  font-weight: normal;
  background-color: #eff2f6;
}
</style>
