<template>
  <div class="card-advertisment">
    <div class="header-advertisment">
      <div class="d-flex item-center justify-content-between">
        <div class="d-flex item-center">
          <Logo />
          <div>
            <div class="header-name">
              <h6>
                <a class="text-advertismenr" href=""
                  >Bootstrap: Font-end framework</a
                >
              </h6>
            </div>
            <p class="mb-0 small">
              Sponsored<el-icon class="icon-sponsor"><WarningFilled /></el-icon>
            </p>
          </div>
        </div>
        <div class="dropdown">
          <a class="nav-link-pills" href=""
            ><el-icon><MoreFilled /></el-icon
          ></a>
        </div>
      </div>
    </div>
    <div class="body">
      <p class="mb-0">
        Quickly design and customize responsive mobile-first sites with
        Bootstrap.
      </p>
    </div>
    <img
      src="https://social.webestica.com/assets/images/post/3by2/02.jpg"
      alt=""
    />
    <div class="footer-advertisment">
      <p>Currently v5.1.3</p>
      <a href="#" class="btn-down">Download now</a>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import Logo from "../Logo/Logo.vue";
export default defineComponent({
  components: {
    Logo,
  },
});
</script>
<style scoped>
.card-advertisment {
  width: 546px;
  background-color: #fff;
  border: 1px solid rgba(0, 0, 0, 0.09);
  border-radius: 0.4rem;
  margin-left: 10px;
}
.header-advertisment {
  padding: 1.25rem 1.25rem;
  border-bottom: 1px solid rgba(0, 0, 0, 0.09);
  display: block;
}
.body {
  padding: 1.25rem 1.25rem;
}
.header:first-child {
  border-radius: calc(0.4rem - 1px) calc(0.4rem - 1px) 0 0;
}

.d-flex {
  display: flex;
  align-items: center;
}
a {
  text-decoration: none;
}
.text-advertismenr {
  color: #14191e;
  font-weight: 700;
  font-size: 0.9375rem;
}
.el-icon {
  vertical-align: -0.123em;
  color: #14191e;
}
.justify-content-between {
  justify-content: space-between;
}
img {
  width: 100%;
}
.footer-advertisment {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1.25rem 1.25rem;
}
.btn-down {
  padding: 0.4rem 0.8rem;
  font-size: 0.8125rem;
  border-radius: 0.2rem;
  font-weight: 500;
  color: #0f6fec;
  background-color: rgba(15, 111, 236, 0.1);
}
.btn-down:hover {
  color: #fff;
  background-color: #0f6fec;
}
.icon-sponsor{
    margin-left: 0.25rem;
}
</style>
