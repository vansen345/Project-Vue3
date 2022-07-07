<template>
  <div class="avatar-status">
    <a href=""
      ><img
        class="img-status rounded border-3 border-white border"
        src="https://social.webestica.com/assets/images/avatar/03.jpg"
        alt=""
    /></a>
  </div>
</template>
<style scoped>
.avatar-status {
  height: 2.1875rem;
  width: 2.1875rem;
  position: relative;
  display: inline-block;
  flex-shrink: 0;
}
.img-status {
  width: 100%;
  height: 100%;
  vertical-align: middle;
  object-fit: cover;
}
.rounded {
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
