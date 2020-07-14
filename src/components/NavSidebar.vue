<template>
  <div id="" class="slide no-slide" v-bind:class="{'show-slide': isSidebarOpen}">
    <div class="">
      <span @click="closeSideBar" class="close-bar"><i class="fa fa-times fa-2x" aria-hidden="true"></i></span>
      <router-link class="link-style" to="/">Home</router-link>
      <router-link class="link-style" to="/about">About Us</router-link>
      <router-link class="link-style" to="/campaigns">Campaigns</router-link>
      <router-link class="link-style" to="/contact">Contact</router-link>
      <div id="donate-btn" class="mx-auto mt-8 box-border link-style flex items-center justify-center cursor-pointer">
        Donate
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavSidebar',
  props: {
    isSidebarOpen: [String, Boolean],
    setSidebarOpen: [String, Function]
  },
  methods: {
    closeSideBar () {
      this.setSidebarOpen(false)
    }
  }
}
</script>

<style scoped>
  #nav-sidebar {
    height: 100vh;
    position: fixed;
    z-index: 1000;
    width: 300px;
    right: -300px;
    background-color: white;
  }
  .link-style {
    font-family: "Cera Pro",serif;
    font-style: normal;
    font-size: 14px;
    font-weight: 500;
    display: block;
    text-align: center;
    padding: 10px 0px;
  }
  #donate-btn {
    border: 2px solid #F18500;
    border-radius: 3px;
    color: #F18500;
    height: inherit;
    width: 126px;
  }

  .close-bar {
    display: block;
    padding-left: 12px;
  }

  @media only screen and (max-width: 767px) {
    .slide {
      padding-top: 30px;
      width: 300px;
      min-width: 200px;
      height: 100vh;
      z-index: 1000;
      position: fixed;
      right: -300px !important;
      background-color: white;
      transition: right 1s;
      border: 1px solid #F18500;
    }
    .show-slide {
      right: 0 !important;
    }
  }
  @media only screen and (min-width: 768px) {
    .no-slide {
      display: none !important;
    }
  }
</style>
