<template>
  <div class="card-profile">
    <div class="card-profile-background">
      <div class="img-background"></div>
      <div class="card-profile-body">
        <div class="text-align-center">
          <avatar-profile />

          <h5 class="mg-0">
            <a href="">Sam Lanson</a>
          </h5>
          <small class="mt-3 text-small">Web Developer at Webestica</small>
          <p>
            I'd love to change the word, but they won't give me the source code
          </p>
          <div class="hastack gap-2">
            <div>
              <h6 class="mg-h6">256</h6>
              <small class="text-small">Post</small>
            </div>
            <div class="vr"></div>
            <div>
              <h6 class="mg-h6">2.5k</h6>
              <small class="text-small">Followers</small>
            </div>
            <div class="vr"></div>
            <div>
              <h6 class="mg-h6">365</h6>
              <small class="text-small">Following</small>
            </div>
          </div>
        </div>
        <hr />
        <ul class="nav-link-secondary flex-column fw-bold gap-2">
          <li class="nav-item">
            <a href="" class="nav-list-profile">
              <img
                class="me-2 h-20px fa-fw"
                src="https://social.webestica.com/assets/images/icon/home-outline-filled.svg"
                alt=""
              />
              <span>Feed</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="" class="nav-list-profile">
              <img
                class="me-2 h-20px fa-fw"
                src="https://social.webestica.com/assets/images/icon/person-outline-filled.svg"
                alt=""
              />
              <span>Connections</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="" class="nav-list-profile">
              <img
                class="me-2 h-20px fa-fw"
                src="https://social.webestica.com/assets/images/icon/earth-outline-filled.svg"
                alt=""
              />
              <span>Lates News</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="" class="nav-list-profile">
              <img
                class="me-2 h-20px fa-fw"
                src="https://social.webestica.com/assets/images/icon/calendar-outline-filled.svg"
                alt=""
              />
              <span>Events</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="" class="nav-list-profile">
              <img
                class="me-2 h-20px fa-fw"
                src="https://social.webestica.com/assets/images/icon/chat-outline-filled.svg"
                alt=""
              />
              <span>Groups</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="" class="nav-list-profile">
              <img
                class="me-2 h-20px fa-fw"
                src="https://social.webestica.com/assets/images/icon/notification-outlined-filled.svg"
                alt=""
              />
              <span>Notifications</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="" class="nav-list-profile">
              <img
                class="me-2 h-20px fa-fw"
                src="https://social.webestica.com/assets/images/icon/cog-outline-filled.svg"
                alt=""
              />
              <span>Settings</span>
            </a>
          </li>
        </ul>
      </div>
      <div class="card-footer text-align-center pa-2">
        <a href="" class="btn-link">View Profile</a>
      </div>
    </div>
    <ul class="list-footer lh-1 mt-1-5 pa-2">
      <li class="nav-item">
        <a href="" class="nav-link-footer"> About </a>
      </li>
      <li class="nav-item">
        <a href="" class="nav-link-footer"> Setting </a>
      </li>
      <li class="nav-item">
        <a href="" class="nav-link-footer color-blue"> Support </a>
      </li>
      <li class="nav-item">
        <a href="" class="nav-link-footer"> Docs </a>
      </li>
      <li class="nav-item">
        <a href="" class="nav-link-footer"> Help </a>
      </li>
      <li class="nav-item">
        <a href="" class="nav-link-footer"> Privacy & terms </a>
      </li>
    </ul>
    <p class="list-footer p-text text-align-center mt-1">
      ©2022

      <a
        class="nav-link-footer pd-0"
        target="_blank"
        href="https://www.webestica.com/"
      >
        Webestica
      </a>
    </p>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import AvatarProfile from "../Avatar/avatarProfile.vue";
export default defineComponent({
  components: {
    AvatarProfile,
  },
});
</script>
<style scoped>
.nav-list-profile:hover {
  color: #0f6fec;
}
p {
  margin-top: 1rem;
  color: #676a79;
}
.hastack {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
}

.vr {
  display: inline-block;
  min-height: 1em;
  width: 1px;
  align-self: stretch;
  /* height: 64px; */
  background-color: currentColor;
  opacity: 0.25;
}
.h-20px {
  height: 20px !important;
}
.me-2 {
  margin-right: 0.6rem !important;
}
.card-profile {
  padding-bottom: 3rem;
}
.mg-0 a {
  text-decoration: none;
  color: #14191e;
  font-family: "Inter", sans-serif;
  font-size: 1.171875rem;
}
.card-profile-background {
  border: 1px solid rgba(0, 0, 0, 0.09);
  border-radius: 0.4rem;
  background-color: #eef0f2;
  overflow: hidden;
  margin-top: 5px;
}
.img-background {
  height: 50px;
  content: "";
  background: gray;
  background-image: url("https://social.webestica.com/assets/images/bg/01.jpg");
  background-position: center;
  background-size: cover;
}
.text-align-center {
  text-align: center;
}
.mg-0 {
  margin-top: 0;
  margin-bottom: 0;
  text-decoration: none;
}
.mt-3 {
  color: rgb(103, 106, 121);
  font-family: var(--bs-body-font-family);
  margin: 2rem auto;
}
.nav-item {
  list-style: none;
  padding: 3px 0;
  margin-right: 5px;
}
.mg-h6 {
  font-family: "Inter", sans-serif;
  font-weight: 700;
  font-size: 0.9375rem;
  color: #14191e;
  margin-bottom: 0;
}
.nav-link-secondary {
  padding-left: 0;
  line-height: 2.3;
}
.nav-list-profile {
  cursor: pointer;
  width: 100%;
  text-decoration: none;
  color: #14191e;
  font-weight: 700;
  font-family: var(--bs-font-sans-serif);
  display: inline-block;
  position: relative;
}
.btn-link {
  padding: 0;
  font-size: 0.8125rem;
  font-weight: 500;
  color: #0f6fec;
  text-decoration: none;
}
.card-footer {
  padding: 0.5rem 0.5rem;
  background: #fff;

  border-top: 1px solid rgba(0, 0, 0, 0.09);
}
.card-profile-body {
  background: white;
  padding: 1.6rem;
  padding-top: 0;
}
hr {
  margin: 1rem 0;
  color: #a1a1a8;
  background-color: currentColor;
  opacity: 0.25;
  border: 1px solid;
  height: 1px;
  border: 0;
}
span {
  font-weight: 700;
}
.list-footer {
  display: flex;
  flex-wrap: wrap;
  padding-left: 0;
  margin-bottom: 0;
  text-align: center;
  justify-content: center;
  font-size: 0.875em;
}
.lh-1 {
  line-height: 1;
}
.mt-1-5 {
  margin-top: 1.5rem;
}
.nav-link-footer {
  text-decoration: none;
  padding: 0.25rem 0.75rem;
  color: #676a79;
  display: block;
}
.nav-link-footer:hover {
  color: #0f6fec;
}
.color-blue {
  color: #0f6fec;
}
.mt-1 {
  margin-top: 0.25rem !important;
}
.p-text {
  gap: 0.5em;
  color: #676a79;
}
.pd-0 {
  padding: 0;
}
img {
  vertical-align: middle;
}
.text-small {
  font-size: 0.875em;
  font-weight: 400;
  color: #676a79;
}
</style>
