<template>
  <div class="avatar avatar-story mr-2">
    <a href=""
      ><img
        class="img-status rounded border-3 border-white border"
        src="https://social.webestica.com/assets/images/avatar/04.jpg"
        alt=""
    /></a>
  </div>
</template>
<style scoped>
.avatar{
    height: 3rem;
    width: 3rem;
    display: inline-block
}
.mr-2{
    margin-right: 0.5rem;
}
.avatar-story {
  position: relative;
  padding: 4px;
  z-index: 1;
}
.avatar-story::after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  border-radius: 50%;
  border: 2px solid #0f6fec;
  z-index: -1;
}
.img-status{
    width: 100%;
    border-radius: 50%;
}

/* .border-white{
  border-color: #fff !important;
  border: 1px solid rgba(0, 0, 0, 0.1) !important;
}
.border{
  border: 1px solid rgba(0, 0, 0, 0.1) !important;
} */
</style>
