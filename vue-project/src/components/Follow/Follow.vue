<template>
  <div class="card-follow">
    <div class="header-follow">
      <h5 class="header-tilte">Who to follow</h5>
    </div>
    <div class="body-follow">
      <div class="infor-follower d-flex mb-1" v-for="item in 3" :key="item">
        <div>
          <AvatarUser />
        </div>
        <div>
          <a class="name-follow" href="#">Judy Nguyen</a>
          <p class="small text-truncate">New anchor</p>
        </div>
        <a href="#" class="btn-primary rounded-circle ms-lg-auto icon-plus"
          ><el-icon><Plus /></el-icon
        ></a>
      </div>
      <div class="infor-follower d-flex mb-1">
        <div>
          <AvatarStory />
        </div>
        <div>
          <a class="name-follow" href="#">Judy Nguyen</a>
          <p class="small text-truncate">New anchorrrrrrrrrr</p>
        </div>
        <a
          href="#"
          class="btn-primary-checked rounded-circle ms-lg-auto icon-plus"
          ><el-icon><Avatar /></el-icon>
        </a>
      </div>
      <div class="view-more d-grid">
        <a href="" class="btn-view-more">View more</a>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import AvatarUser from "../Avatar/avatarUser.vue";
import AvatarStory from "../Avatar/avtarStory.vue";
import { defineComponent } from "vue";
export default defineComponent({
  components: {
    AvatarUser,
    AvatarStory,
  },
});
</script>
<style scoped>
.card-follow {
  width: 261px;
  background-color: #fff;
  border: 1px solid rgba(0, 0, 0, 0.09);
  border-radius: 0.4rem;
  border-top-color: rgba(0, 0, 0, 0.09);
}
.header-follow {
  padding: 1.25rem 1.25rem 0;
}
h5,
.name-follow {
  font-family: "Inter", sans-serif;
  font-weight: 700;
  line-height: 1.25;
  color: #14191e;
}
.header-tilte {
  font-size: 1.171875rem;
}
.body-follow {
  padding: 1.25rem;
}
a {
  text-decoration: none;
}
.d-flex {
  display: flex;
}
.mb-1 {
  margin-bottom: 1rem;
}
.text-truncate {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
  width: 100px;
}
.small {
  font-size: 0.875em;
}
.btn-primary,
.btn-primary-checked {
  height: 2.5rem;
  width: 2.5rem;
  font-size: 0.9em;
  color: #0f6fec;
  background-color: rgba(15, 111, 236, 0.1);
}
.btn-primary-checked {
  color: #fff;
  background-color: #0f6fec;
  border-color: #0f6fec;
}
.rounded-circle {
  border-radius: 50%;
}
.ms-lg-auto {
  margin-left: auto;
}
.icon-plus {
  display: inline-flex;
  align-items: center;
  justify-content: center;
}
.btn-view-more {
  padding: 0.4rem 0.8rem;
  font-size: 0.8125rem;
  border-radius: 0.2rem;
  color: #0f6fec;
  background-color: rgba(15, 111, 236, 0.1);
  text-align: center;
}
.btn-view-more:hover {
  color: #fff;
  background-color: #0f6fec;
}
.d-grid {
  display: grid;
}
.name-follow:hover {
  color: #0c59bd;
}
.icon-plus:hover {
  color: #fff;
  background-color: #0f6fec;
}
</style>
