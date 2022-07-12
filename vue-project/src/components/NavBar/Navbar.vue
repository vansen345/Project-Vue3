<template>
  <div class="collapse">
    <a href="" class="nav-brand">
      <img
        class="img-logo"
        src="https://social.webestica.com/assets/images/logo.svg"
        alt=""
      />
    </a>

    <div class="menu">
      <div class="nav">
        <div class="nav-item">
          <form class="rounded position-relative">
            <input
              type="search"
              class="form-control pe-3"
              placeholder="Search....."
            />
            <button class="position-absolute border-0 background-transparent">
              <Search
                style="
                  width: 1em;
                  height: 1em;
                  font-size: 1.171875rem;
                  color: #696c7b;
                "
              />
            </button>
          </form>
        </div>
      </div>
      <ul class="list-navbar">
        <li class="list-navbar-item nav-item-dropdown">
          <a class="nav-link active dropdown-toggle"
            >Demo<el-icon class="icon-arrowdown"><ArrowDownBold /></el-icon>
          </a>

          <ul class="dropdown-menu">
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item active">Home default</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Home classic </a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Home post</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Home video</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Home event</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Landing page</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">App download</a>
            </li>
            <li class="dropdown-driver"></li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item"
                ><el-icon class="me-2"><Download /></el-icon>Buy social!</a
              >
            </li>
          </ul>
        </li>
        <li class="list-navbar-item nav-item-dropdown">
          <a class="nav-link dropdown-toggle"
            >Pages <el-icon class="icon-arrowdown"><ArrowDownBold /></el-icon
          ></a>

          <ul class="dropdown-menu">
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Albums</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Celebration </a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Messaging</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Profile</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Events</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Events 2</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Event details</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Event details 2</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Groups</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Group details</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Post video</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Post video details</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Post details</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Video details</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Blog</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Blog details</a>
            </li>
          </ul>
        </li>
        <li class="list-navbar-item nav-item-dropdown">
          <a class="nav-link dropdown-toggle"
            >Account <el-icon class="icon-arrowdown"><ArrowDownBold /></el-icon
          ></a>
          <ul class="dropdown-menu">
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Create a page</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Settings </a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Notifications</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Helper center</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Help details</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Authentications</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Error 404</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Offline</a>
            </li>
            <li class="dropdown-menu-list">
              <a href="" class="dropdown-item">Privacy & terms</a>
            </li>
          </ul>
        </li>
        <li class="list-navbar-item nav-item-dropdown">
          <a class="nav-link">My Netword</a>
        </li>
      </ul>
    </div>
    <div class="notification">
      <a href="" class="btn-light border-radius">
        <el-icon class="icon-md"><ChatLineSquare /></el-icon>
      </a>

      <a href="" class="btn-light border-radius"
        ><el-icon class="icon-md"> <Setting /> </el-icon
      ></a>

      <a href="" class="btn-light border-radius"
        ><span class="circle-notif"></span
        ><el-icon class="icon-md"><BellFilled /></el-icon
      ></a>

      <AvatarProfile />
    </div>
  </div>
</template>

<script lang="ts">
import { Search } from "@element-plus/icons-vue";
import { defineComponent, ref } from "vue";
import { ElButton, ElInput, ElMenu } from "element-plus";
import { BellFilled } from "@element-plus/icons-vue";
import AvatarProfile from "../Avatar/avatarProfile.vue";
export default defineComponent({
  components: {
    ElButton,
    ElInput,
    ElMenu,
    BellFilled,
    AvatarProfile,
    Search,
  },
  setup() {
    const activeIndex = ref("1");
    const activeIndex2 = ref("1");
    const handleSelect = (key: string, keyPath: string[]) => {
      console.log(key, keyPath);
    };
  },
});
</script>

<style scoped>
.nav-link.active {
  color: #0f6fec;
}
.collapse {
  display: flex;
  align-items: center;
  width: 1140px;
  margin-left: auto;
  margin-right: auto;
  flex: 0 0 auto;
  padding-left: 12px;
  padding-right: 12px;
}
.btn-light {
  background-color: #eef0f2;
  border: 0;
  width: 2.5rem;
  height: 2.5rem;
  margin-right: 0.5rem;
  display: flex;
  align-items: center;
  justify-content: center;
}
.border-radius {
  border-top-left-radius: 0.4rem;
  border-bottom-left-radius: 0.4rem;
  border-top-right-radius: 0.4rem;
  border-bottom-right-radius: 0.4rem;
}
.notification {
  margin: 10px;
  display: flex;
}

.menu {
  display: flex;
  flex-grow: 1;
}
.btn-collapse {
  display: flex;

  margin: 10px;
}
.icon-md {
  font-size: 0.9375rem;
  color: #676a79;
}
.form-control {
  border: 0;
  width: 100%;
  padding: 0.7rem 1rem;
  border-radius: 5px;
  margin-left: 20px;
  border: 1px solid rgba(0, 0, 0, 0.1);
  background-color: rgb(238, 240, 242);
}
.list-navbar {
  display: flex;
  list-style: none;
  margin-left: auto;
  padding-left: 0;
  margin-right: 10px;
}
.nav-link {
  padding-left: 2rem;
  padding-right: 0rem;
  cursor: pointer;
  font-size: 0.9375rem;
  font-weight: 600;
  text-transform: capitalize;
  line-height: 40px;
  padding-top: 0;
  padding-bottom: 0;
  color: #676a79;
}
.list-navbar-item:hover > .dropdown-menu {
  visibility: visible;
  opacity: 1;
  z-index: 1;
  transform: translateY(0%);
  transition-delay: 0s, 0s, 0.3s;
}
.nav-link:hover {
  color: #0f6fec;
}
.dropdown-menu {
  visibility: hidden;
  flex-direction: column;
  background-color: #fff;
  text-align-last: start;
  position: absolute;
  list-style: none;
  border-radius: 0.4rem;
  border: 1px solid rgba(0, 0, 0, 0.06);
  padding: 0.5rem 0;
  background-clip: padding-box;
  transform: translateY(1em);
  opacity: 0;
  z-index: -1;
  transition: all 0.3s ease-in-out 0s, visibility 0s linear 0.3s,
    z-index 0s linear 0.01s;
  min-width: 15rem;
}
.dropdown-menu-list {
  padding: 6.4px 19.2px;
}
.dropdown-item {
  width: 100%;
  font-family: var(--bs-body-font-family);
  font-weight: 500;
  color: #676a79;
  text-align: inherit;
  white-space: nowrap;
  background-color: transparent;
  border: 0;
  text-decoration: none;
  font-size: var(--bs-body-font-size);
}
.circle-notif {
  width: 8px;
  height: 8px;
  background: #d6293e;
  border-radius: 50%;
  position: absolute;
  top: 0;
  right: 0;
}
.btn-primary {
  width: 2.5rem;
  height: 36px;
  background: #0f6fec;
  border-color: #0f6fec;
}
.avt-user {
  margin-top: 0px;
  margin-left: 10px;
}
.icon-arrowdown {
  vertical-align: middle;
  font-size: 0.5rem;
  margin-left: 0.35rem;
}
.el-input--large {
  margin-left: 2rem;
}
.el-input__wrapper {
  background: rgb(238, 240, 242);
  opacity: 1;
}
.rounded {
  border-radius: 0.4rem;
}
.position-relative {
  position: relative;
}
.position-absolute {
  position: absolute;
  top: 20%;
  left: 10%;
}
.pe-3 {
  padding-left: 3rem;
}
.border-0 {
  border: 0;
  cursor: pointer;
}
.background-transparent {
  background: transparent;
}
.dropdown-driver {
  height: 0;
  margin: 0.5rem 0;
  overflow: hidden;
  border-top: 1px solid rgba(0, 0, 0, 0.1);
}
.me-2 {
  margin-right: 0.5rem;
  color: #0cbc87;
}
.dropdown-item:hover {
  color: #0f6fec;
}
.dropdown-item.active {
  color: #0f6fec;
}
.icon-md:hover {
  color: #0c59bd;
}
.img-logo {
  display: block;
  width: 36px;
  height: 36px;
}
</style>
