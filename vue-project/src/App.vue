<script lang="ts">
import { defineComponent } from "vue";
import { ElContainer, ElHeader, ElMain } from "element-plus";
import Navbar from "./components/NavBar/Navbar.vue";
import Profile from "./components/Profile/Profile.vue";
import Story from "./components/Story/storyComponent.vue";
import PostStatus from "./components/PostStatus/PostStatus.vue";
import FirstNews from "./components/News/firstNews.vue";

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
  },
});
</script>

<template>
  <el-container class="container">
    <el-header class="header">
      <navbar />
    </el-header>
    <div class="body">
      <div class="container">
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
.container {
  width: 100%;
  display: flex;
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
  margin-left: 5rem;
  flex: 0 0 259px;
  margin-top: 1.6rem;
}
#app {
  width: 100%;
  font-weight: normal;
  background-color: #eff2f6;
  color: #676a79;
}
</style>
