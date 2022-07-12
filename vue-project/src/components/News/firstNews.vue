<template>
  <div class="card-first-news">
    <div class="card-headers-news pd-0">
      <div class="d-flex item-center justify-content-between">
        <div class="d-flex item-center">
          <AvatarStory />
          <div>
            <div class="header-name">
              <h6>
                <a class="text-header" href="">Lori Ferguson</a>
              </h6>
              <span class="nav-item-small d-flex item-center">2hr</span>
            </div>
            <p class="mb-0 small">Web Developer at Webestica</p>
          </div>
        </div>
        <div class="dropdown">
          <a class="nav-link-pills" href=""
            ><el-icon><MoreFilled /></el-icon
          ></a>
        </div>
      </div>
    </div>
    <div class="card-body-news">
      <p class="mb-1">
        I'm thrilled to share that I've completed a graduate certificate course
        in project management with the president's honor roll.
      </p>
      <img
        class="card-body-img border-top-bottom"
        src="https://social.webestica.com/assets/images/post/3by2/01.jpg"
        alt=""
      />
      <ul class="d-flex pd-1 gap-0">
        <li class="nav-item">
          <a class="nav-link active" href=""
            ><el-icon class="pe-1"><ChatRound /></el-icon
            ><span class="pe-2">Liked (56)</span></a
          >
        </li>
        <li class="nav-item">
          <a class="nav-link" href=""
            ><el-icon class="pe-1"><ChatRound /></el-icon
            ><span class="pe-2">Comments (12)</span></a
          >
        </li>
        <li class="nav-item mg-le-auto">
          <a class="nav-link" href=""
            ><el-icon class="no-inherit">
              <Share />
            </el-icon>
            <span class="pe-2">Share (3)</span></a
          >
        </li>
      </ul>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import AvatarStory from "../Avatar/avtarStory.vue";
export default defineComponent({
  components: {
    AvatarStory,
  },
});
</script>
<style scoped>
.card-first-news {
  width: 546px;
  background-color: #fff;
  border: 1px solid rgba(0, 0, 0, 0.09);
  border-radius: 0.4rem;
  margin-left: 10px;
}
.nav-item {
  list-style: none;
}
.nav-link:hover {
  color: #0f6fec;
}
.card-headers-news,
.card-body-news {
  padding: 1.25rem 1.25rem;
}
.header-name {
  display: flex;
}
h6 {
  font-size: 0.9375rem;
}
.pd-0 {
  padding-bottom: 0;
}
a {
  text-decoration: none;
}
.text-header {
  color: #14191e;
  font-weight: 700;
}
.nav-item-small,
.small,
.nav-link {
  font-weight: 400;
  color: #676a79;
  font-size: 0.875em;
}
.nav-item-small::before {
  content: "•";
  color: inherit;
  padding-left: 0.6rem;
  padding-right: 0.6rem;
  opacity: 0.8;
}
.d-flex {
  display: flex;
  align-items: center;
}
.justify-content-between {
  justify-content: space-between;
}
.border-top-bottom {
  border-bottom-right-radius: calc(0.4rem - 1px);
  border-bottom-left-radius: calc(0.4rem - 1px);
  border-top-left-radius: calc(0.4rem - 1px);
  border-top-right-radius: calc(0.4rem - 1px);
}
.card-body-img {
  width: 100%;
}
.mb-1 {
  margin-bottom: 1rem;
}
.pd-1 {
  padding: 1rem 0 1rem 0rem;
}
.el-icon {
  vertical-align: -0.123em;
}
.pe-2 {
  padding-left: 0.25rem;
}
.nav-link.active {
  color: #0f6fec;
}
.gap-0 {
  gap: 0.7rem;
}
.mg-le-auto {
  margin-left: auto;
}
.nav-link-pills:hover {
  background-color: rgba(20, 25, 30, 0.1);
}
.nav-link-pills {
  color: black;
  padding: 0.25rem 0.5rem;
  border-radius: 0.4rem;
}
</style>
