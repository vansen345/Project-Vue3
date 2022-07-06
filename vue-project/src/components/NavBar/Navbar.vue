<template>
  <div class="collapse">
    <div class="btn-collapse">
      <el-button type="primary" class="btn-primary" />
      <input type="search" class="form-control" />
    </div>
    <div class="menu">
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
                ><i class="text-success fa-solid fa-cloud-arrow-down"></i>Buy
                social!</a
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
      <el-button type="Info" class="btn-light"
        ><el-icon><ChatDotSquare /></el-icon
      ></el-button>
      <el-button type="Info" class="btn-light"
        ><el-icon><Setting /></el-icon
      ></el-button>
      <el-button type="Info" class="btn-light"
        ><span class="circle-notif"></span><el-icon><BellFilled /></el-icon
      ></el-button>

      <avartar-user class="avt-user" />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";
import { ElButton, ElInput, ElMenu } from "element-plus";
import { BellFilled } from "@element-plus/icons-vue";
import avartarUser from "../Avatar/avatarUser.vue";
export default defineComponent({
  components: {
    ElButton,
    ElInput,
    ElMenu,
    BellFilled,
    avartarUser,
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
  justify-content: space-around;
  margin-left: 3rem;
  flex: 0 0 auto;
}
.btn-light {
  background-color: #eef0f2;
  border: 0;
  width: 2.5rem;
  height: 2.5rem;
}
.notification {
  margin: 10px;
  display: flex;
}
.menu {
  display: flex;
  margin-left: 7rem;
}
.btn-collapse {
  display: flex;

  margin: 10px;
}

.form-control {
  border: 0;
  width: 100%;
  padding: 0.5rem 1rem;
  border-radius: 5px;
  margin-left: 20px;
  border: 1px solid rgba(0, 0, 0, 0.1);
}
.list-navbar {
  display: flex;
  list-style: none;
  margin: 10px;
}
.nav-link {
  padding-left: 3rem;
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
.nav-link:hover + .dropdown-menu {
  visibility: visible;
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
  border-radius: 5px;
  /* margin: 0; */
  margin: 5px auto;
  border: 1px solid rgba(0, 0, 0, 0.06);
  padding: 2rem 0;
  background-clip: padding-box;
  z-index: 1;
}
.dropdown-item {
  width: 100%;
  padding: 0.4rem 1.2rem;
  font-family: var(--bs-body-font-family);
  font-weight: 400;
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
  top: -10px;
  right: -15px;
}
.btn-primary {
  width: 2.5rem;
  height: 2.5rem;
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
</style>
