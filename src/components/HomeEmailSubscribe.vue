<template>
  <div class="w-full" style="">
    <div class="w-1/3 m-auto text-center" style="margin-bottom: 56px">
      <h3>You Too Can Make A Difference</h3>
      <span>Subscribe to our newsletter to stay informed about our news and upcoming events.</span>
    </div>
    <div class="w-1/3 md:flex m-auto">
      <input class="flex-1  w-full outline-none focus:bg-yellow-100 focus:border-4 focus:border-yellow-500"/>
      <button class="mx-auto md:mx-0 p-2">Subscribe</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeEmailSubscribe'
}
</script>

<style scoped>
  h3 {
    font-family: Cera Pro,serif;
    font-style: normal;
    font-weight: 900;
    font-size: 28px;
    line-height: 35px;
    color: #FFFFFF;
    margin-bottom: 20px;
  }
  span {
    font-family: "Cera Pro",sans-serif;
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 150%;
    color: #FFFFFF;
    margin-bottom: 30px;
  }
  button {
    background-color: #F18500;
    border: 1px solid #FFFFFF;
    color: #FFFFFF;
  }
  input {
    font-size: 26px;
  }
</style>
