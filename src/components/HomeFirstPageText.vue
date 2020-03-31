<template>
  <div>
    <h3><strong>A world where every one is</strong></h3>
    <h3><strong>given a chance to live</strong></h3>
    <span>We aim to bridge the gap and lorem towards the sustainable development goals</span>
    <div id="donate-btn" class="flex items-center justify-center cursor-pointer">
      Donate To Our Cause
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeFirstPageText'
}
</script>

<style scoped>
h3 {
  font-family: Cera Pro,serif;
  font-style: normal;
  font-weight: 900;
  font-size: 40px;
  line-height: 120%;
}
span {
  display: inline-block;
  font-family: "Cera Pro",serif;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 20px;
  margin: 20px 0;
  width: 75%;
  color: #141414;
}
#donate-btn {
  background-color: #F18500;
  color: white;
  width: 200px;
  height: 40px;
  font-family: "Cera Pro",serif;
  font-style: normal;
}
</style>
