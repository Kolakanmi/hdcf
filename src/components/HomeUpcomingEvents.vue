<template>
  <div>
    <div class="m-auto text-center md:w-2/5" style="margin-bottom: 100px">
      <h3 class=""><strong>Upcoming Campaigns</strong></h3>
      <span>We aim to bridge the gap and lorem towards the sustainable development goals.</span>
    </div>
    <div class="flex">
      <div class="my-auto ml-2 mr-20">
        <p class="flex mb-2 mx-auto cursor-pointer" style="background-color: #F18500; border-radius: 50%; width: 30px; height: 30px">
          <img class="m-auto" alt="left-arrow"  src="../../images/left-arrow.svg">
        </p>
        <p class="flex mb-2 mx-auto cursor-pointer" style="background-color: #F18500; border-radius: 50%; width: 30px; height: 30px">
          <img class="m-auto" alt="right-arrow" src="../../images/right-arrow.svg">
        </p>
      </div>
      <div class="flex w-8/12">
        <HomeCountdownCard/>
      </div>
    </div>
  </div>
</template>

<script>
import HomeCountdownCard from '@/components/HomeCountdownCard'
export default {
  name: 'HomeUpcomingEvents',
  components: { HomeCountdownCard }
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
</style>
