<template>
  <div class="avatar-profile">
    <a href=""
      ><img
        class="img-profile rounded border-3 border-white border"
        src="https://social.webestica.com/assets/images/avatar/07.jpg"
        alt=""
    /></a>
  </div>
</template>
<style scoped>
.avatar-profile {
  width: 4rem;
  height: 4rem;
  position: relative;
  display: inline-block;
  flex: 0 0 3rem;
}
.img-profile {
  width: 100%;
  height: 100%;

  margin-top: -1rem;
  border: solid white;
  object-fit: cover;
}
.rounded {
  border-radius: 0.4rem !important;
}
.border-3 {
  border-width: 3px;
  border-color: white;
}
/* .border-white{
  border-color: #fff !important;
  border: 1px solid rgba(0, 0, 0, 0.1) !important;
}
.border{
  border: 1px solid rgba(0, 0, 0, 0.1) !important;
} */
</style>
