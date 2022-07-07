<template>
  <div class="arrow-hover">
    <div class="story-slider">
      <div class="tns1-mw">
        <div class="tiny-slider">
          <div class="tns-slider">
            <div class="inner inner-item1">
              <a href="#" class="icon-plus-story"
                ><el-icon><Plus /></el-icon>
              </a>
              <h6 class="mt-2 text-h6">Post a story</h6>
            </div>
            <div class="inner inner-item-2" v-for="item in 4" :key="item">
              <div class="img-story">
                <div class="story-content">
                  <a href="" class="name-user">Judy Nguyensasdwddffffdsfdsfs</a>
                </div>
              </div>
            </div>
          
          </div>
        </div>
      </div>
      <div class="tns-controls" tabindex="0">
        <button
          type="button"
          class="btn-prev"
          data-controls="prev"
          tabindex="-1"
        >
          <el-icon><ArrowLeft /></el-icon>
        </button>
        <button
          type="button"
          class="btn-next"
          data-controls="next"
          tabindex="-1"
        >
          <el-icon><ArrowRight /></el-icon>
        </button>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import { ElImage } from "element-plus";

export default defineComponent({
  components: {
    ElImage,
  },
  data(){
    return{
      name_user:''
    }
  }
});
</script>
<style scoped>
.story-slider {
  width: 546px;
  position: relative;
}
.tns1-mw {
  width: 546px;
}
.tns-slider {
  width: 747px;
}
.img-story {
  position: absolute;
  bottom: 0;
  width: 112px;
}
.story-content {
  margin: 4px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  width: 104px;
  color: white;
}
.arrow-hover {
  width: 546px;
  overflow: hidden;
}
.tns-controls [data-controls] {
  position: absolute;
  top: 50%;
  width: 30px;
  height: 30px;
  display: block;
  line-height: 30px;
  transition: all 0.3s ease-in-out;
  background: rgba(15, 111, 236, 0.3);
  color: #fff;
  border: none;
  padding: 0;
  margin: 0 5px;
  z-index: 9;
  transform: translateY(-300%);
  border-radius: 0.4rem;
}
.tns-controls [data-controls="prev"] {
  left: -60px;
}
.tns-controls [data-controls="next"] {
  right: -60px;
}
.arrow-hover:hover [data-controls="prev"] {
  left: 0;
}
.arrow-hover:hover [data-controls="next"] {
  right: 0;
}
.tns-controls [data-controls]:hover {
  cursor: pointer;
  background-color: #0f6fec;
}

.inner {
  background-color: white;
  position: relative;
  width: 112px;
  border-radius: 0.4rem;
  display: inline-block;
  margin-left: 15px;
  height: 150px;
}
.icon-plus-story {
  height: 2.5rem;
  width: 2.5rem;
  font-size: 0.9em;
  display: inline-flex;
  margin-top: 10px;
  align-items: center;
  justify-content: center;
  background-color: #eef0f2;
  border-color: #eef0f2;
  border-radius: 50%;
  color: #000;
}
.inner-item1 {
  border-style: dashed !important;
  border: 1px solid rgba(0, 0, 0, 0.09);
  border-width: 2px !important;
  display: inline-flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  vertical-align: top;
}
.inner-item-2,
.inner-item-3,
.inner-item-4 {
  content: "";
  background: gray;
  background-image: url("https://social.webestica.com/assets/images/post/1by1/02.jpg");
  background-position: center left;
  background-size: cover;
}
.inner-item-3 {
  background-image: url("https://social.webestica.com/assets/images/post/1by1/02.jpg");
}
.inner-item-4 {
  background-image: url("https://social.webestica.com/assets/images/post/1by1/02.jpg");
}
.name-user {
  color: rgb(255, 255, 255);
  font-size: 0.875em;
  text-decoration: none;
}
.text-h6 {
  font-size: 0.875em;
  margin-top: 0.5rem;
  color: #14191e;
}
</style>
