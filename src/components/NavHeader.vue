<template>
  <div id="nav-header" class="flex">
    <div style="height: 68px; width: 125.09px;" class="my-auto">
      <img alt="logo" src="../../images/logo.png" />
    </div>
    <div id="nav" class="box-content hidden sm:flex my-auto ml-auto justify-end lg:w-3/4">
      <router-link class="link-style my-auto" to="/">Home</router-link>
      <router-link class="link-style my-auto" to="/about">About Us</router-link>
      <router-link class="link-style my-auto" to="/campaigns">Campaigns</router-link>
      <router-link class="link-style my-auto" to="/contact">Contact</router-link>
      <div id="donate-btn" class="box-border link-style flex items-center justify-center cursor-pointer">
        Donate
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'NavHeader'
}
</script>

<style scoped>
#nav-header {
  margin: 0;
  padding: 0;
  //border: 2px solid blue;
}
#nav {
  height: 40px;
  //border: 2px solid blue;
}
#donate-btn {
  border: 2px solid #F18500;
  border-radius: 3px;
  color: #F18500;
  height: inherit;
  width: 126px;
}
.link-style {
  font-family: "Cera Pro",serif;
  font-style: normal;
  font-size: 14px;
  font-weight: 500;
  margin-left: 20px;
  margin-right: 20px;
}
</style>
