<script lang="ts">
import { defineComponent } from "vue";
import { ElContainer, ElHeader, ElMain } from "element-plus";
import Navbar from "./components/NavBar/Navbar.vue";
import Profile from "./components/Profile/Profile.vue";
import Story from "./components/Story/Story.vue";
import PostStatus from "./components/PostStatus/PostStatus.vue";
import FirstNews from "./components/News/FirstNews.vue";
import Advertisment from "./components/Advertisement/Advertisement.vue";
import Follow from "./components/Follow/Follow.vue";
import TodayNews from "./components/TodayNews/TodayNews.vue";

export default defineComponent({
  components: {
    ElContainer,
    ElHeader,
    ElMain,
    Navbar,
    Profile,
    Story,
    PostStatus,
    FirstNews,
    Advertisment,
    Follow,
    TodayNews,
  },
});
</script>

<template>
  <el-container class="container">
    <el-header class="header position-fixed">
      <div class="navbar">
        <div class="row-header">
          
          <Navbar />
        </div>
      </div>
    </el-header>
    <div class="body">
      <div class="container-body">
        <div class="row">
          <div class="profile">
            <Profile />
          </div>
          <div class="news">
            <div>
              <Story />
            </div>
            <div>
              <PostStatus />
            </div>
            <div>
              <FirstNews />
            </div>
            <div>
              <Advertisment />
            </div>
          </div>
          <div class="follow">
            <div>
              <Follow />
            </div>
            <div>
              <TodayNews />
            </div>
          </div>
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
.position-fixed {
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  z-index: 1030;
}
.navbar {
  width: 1351px;
  display: flex;
}
.header {
  background: white;
  padding: 0;
  width: 1351px;
  height: 56px;
}
.row-header {
  width: 1351px;
  display: flex;
 
}
.body {
  width: 100%;
  height: 100%;
  padding-top: calc(1.5rem + 35px);
}
.container-body {
  width: 1140px;
  padding-bottom: 1rem;
  margin-left: auto;
  margin-right: auto;
  padding-left: 12px;
}
.news {
  width: 570px;
  margin-top: 2rem;
  padding-left: 12px;
  gap: 1.5rem;
  display: flex;
  flex-direction: column;
}
.profile {
  width: 259px;

  flex: 0 0 259px;
  margin-top: 1.6rem;
}
.row {
  display: flex;
  width: 1140px;
}
.follow {
  width: 285px;
  flex: 0 0 auto;
  padding-left: 1rem;
  margin-top: 2rem;
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}
#app {
  width: 100%;
  font-weight: normal;
  background-color: #eff2f6;
  color: #676a79;
}
</style>
