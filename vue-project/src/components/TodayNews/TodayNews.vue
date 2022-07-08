<template>
  <div class="today-news">
    <div class="header-news">
      <h5 class="tilte-new">Today's news</h5>
    </div>
    <div class="body-news">
      <div class="first-new" v-for="item in 4" :key="item">
        <h6 class="tiltle-hover">Ten question you should answer truthfully</h6>
        <small>2hr</small>
      </div>
      <a href="" class="btn-link-loader d-flex">
        <div class="spinner-dots mr-2">
          <span class="spinner-dot"></span>
          <span class="spinner-dot"></span>
          <span class="spinner-dot"></span>
        </div>
        View all latest news
      </a>
    </div>
  </div>
</template>
<style scoped>
.today-news {
  width: 261px;
  background-color: #fff;
  border-radius: 0.4rem;
}
.header-news {
  padding: 1.25rem 1.25rem 0;
}
.body-news {
  padding: 1.25rem;
}
.tilte-new {
  font-size: 1.171875rem;
}
h5,
h6 {
  font-family: "Inter", sans-serif;
  font-weight: 700;
  line-height: 1.25;
  color: #14191e;
}
h6 {
  font-size: 0.9375rem;
}
a {
  text-decoration: none;
}
.first-new {
  margin-bottom: 1rem;
}
.d-flex{
    display: flex;
}
.spinner-dot {
  background-color: #a1a1a8;
  display: inline-block;
  height: 4px;
  margin: 2px;
  border-radius: 50%;
  width: 4px;
}
.mr-2{
    margin-right: 0.5rem;
}
.btn-link-loader{
    font-size: 0.875em;
    color: rgb(20, 25, 30);
    font-weight: 500;
}
.tiltle-hover:hover{
    color: #0c59bd;;
}
.tiltle-hover{
    cursor: pointer;
}
</style>
