<template>
  <div class="card-post-status">
    <div class="content-post">
      <AvatarUser />
      <form class="form-post" action="">
        <textarea
          class="form-control pe-4 border-0"
          rows="2"
          ref="textarea"
          @focus="resize"
          @keyup="resize"
          data-autoresize=""
          placeholder="Share your thoughts..."
        ></textarea>
      </form>
    </div>
    <ul class="nav-pill fw-500">
      <li class="nav-item">
        <a class="nav-link-pills" href=""
          ><el-icon class="el-icon icon-photo"><PictureFilled /></el-icon
          ><span>Photo</span></a
        >
      </li>
      <li class="nav-item">
        <a class="nav-link-pills" href=""
          ><el-icon class=" el-icon icon-video"><VideoCameraFilled /></el-icon
          ><span>Video</span></a
        >
      </li>
      <li class="nav-item">
        <a class="nav-link-pills" href=""
          ><el-icon class="el-icon icon-even"><Calendar /></el-icon
          ><span>Event</span></a
        >
      </li>
      <li class="nav-item">
        <a class="nav-link-pills" href=""
          ><el-icon class="el-icon icon-feeling"><VideoCameraFilled /></el-icon
          ><span>Feeling /Activity</span></a
        >
      </li>
      <li class="nav-item mg-l-auto">
        <a class="nav-link-pills" href=""
          ><el-icon><MoreFilled /></el-icon
        ></a>
      </li>
    </ul>
  </div>
</template>
<style scoped>
.card-post-status {
  width: 546px;
  position: relative;
  border-radius: 0.4rem;
  background-color: #fff;
  border: 1px solid rgba(0, 0, 0, 0.09);
  padding: 1.25rem 1.25rem;
  margin-left: 10px;
}
.form-post {
  width: 100%;
}
.content-post {
  display: flex;
  width: 504px;
  margin-bottom: 1rem;
}
.form-control {
  resize: none;
  overflow: hidden;
  min-height: 80px;
}
.border-0 {
  border: none;
  outline: none;
}
.pe-4 {
  padding: 0.5rem 1.5rem;
}
textarea {
  font-family: inherit;
  font-size: 0.9375rem;
  font-weight: 400;
  color: #29292e;
}
.nav-pill {
  display: flex;
  flex-direction: row;
  gap: 0.7rem;
  font-size: 0.875em;
  padding-left: 0;
}
.nav-item {
  list-style: none;
}
.nav-link-pills {
  text-decoration: none;
  background: rgba(238, 240, 242);
  padding: 0.35rem 0.6rem;
  border: 0;
  border-radius: 0.4rem;
  color: #676a79;
}
span {
  font-weight: 500;
  margin-left: 5px;
}
.el-icon {
  vertical-align: -0.123em;
}
.icon-photo {
  color: rgba(12, 188, 135);
}
.icon-video {
  color: rgba(79, 158, 248);
}
.icon-even {
  color: rgba(214, 41, 62);
}
.icon-feeling {
  color: rgba(247, 195, 46);
}
.mg-l-auto {
  margin-left: auto;
}
.nav-link-pills:hover {
  color: #0c59bd;
}
</style>
<script lang="ts">
import { defineComponent } from "vue";
import AvatarUser from "../Avatar/avatatStatus.vue";

export default defineComponent({
  components: {
    AvatarUser,
  },
  mounted(){
      this.resize();

  },
  methods:{
    resize(){
      const {textarea} = this.$refs;
      textarea.style.height = textarea.scrollHeight - 4 + 'px';
    }
  },
 
});
</script>
