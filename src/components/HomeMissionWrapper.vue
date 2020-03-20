<template>
  <div id="mission-wrapper" class="">
    <div id="mission" class="m-auto text-center md:w-2/5">
      <h3 class=""><strong>Our Mission</strong></h3>
      <span>We aim to bridge the gap and lorem towards the sustainable development goals.</span>
    </div>
    <div class="md:flex" style="margin-top: 100px">
      <div class="md:flex-auto mr-24 mb-24">
        <span class="mission-image"><img alt="bulb" src="../../images/bulb.svg"/></span>
        <h4 class="mission-h4"><strong>Education</strong></h4>
        <span>We aim to bridge the gap and lorem towards the sustainable development goals.</span>
      </div>
      <div class="md:flex-auto mr-24 mb-24">
        <span class="mission-image"><img alt="heart" src="../../images/heart.svg"/></span>
        <h4 class="mission-h4"><strong>Medicals</strong></h4>
        <span>We aim to bridge the gap and lorem towards the sustainable development goals.</span>
      </div>
      <div class="md:flex-auto">
        <span class="mission-image"><img alt="earth" src="../../images/earth.svg"/></span>
        <h4 class="mission-h4"><strong>Healthy Food</strong></h4>
        <span>We aim to bridge the gap and lorem towards the sustainable development goals.</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeMissionWrapper'
}
</script>

<style scoped>
  h3 {
    font-family: Cera Pro,serif;
    font-style: normal;
    font-size: 28px;
    line-height: 35px;
    margin-bottom: 20px;
    color: #141414;
  }
  span {
    display: inline-block;
    font-family: "Cera Pro",serif;
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 150%;
    color: #565050;
  }
  .mission-image {
    margin-bottom: 30px;
    height: 50px;
    width: 50px;
  }
  .mission-h4 {
    margin-bottom: 20px;
    font-family: Cera Pro,serif;
    font-style: normal;
    font-size: 20px;
    line-height: 25px;
    color: #141414;
  }
</style>
