<template>
  <div>
    <div class="m-auto text-center md:w-2/5" style="margin-bottom: 100px">
      <h3 class=""><strong>Upcoming Campaigns</strong></h3>
      <span>We aim to bridge the gap and lorem towards the sustainable development goals.</span>
    </div>
    <div class="flex" style="padding-left: 13.68%;">
      <div class="my-auto ml-0 md:ml-2 mr-8 md:mr-20">
        <p @click="handleScrollLeft" class="flex mb-8 mx-auto cursor-pointer" style="background-color: #F18500; border-radius: 50%; width: 30px; height: 30px">
          <img class="m-auto" alt="left-arrow"  src="../../images/left-arrow.svg">
        </p>
        <p @click="handleScrollRight" class="flex mx-auto cursor-pointer" style="background-color: #F18500; border-radius: 50%; width: 30px; height: 30px">
          <img class="m-auto" alt="right-arrow" src="../../images/right-arrow.svg">
        </p>
      </div>
      <div ref="scrollerCards" class="flex p-1 w-full flex-no-wrap overflow-x-hidden">
        <HomeCountdownCard event-image="children-sitting.png" location="Ikoyi Orphanage" date="July 18, 2020"/>
        <HomeCountdownCard event-image="home-event2.svg" location="Lekki Orphanage" date="August 20, 2020"/>
      </div>
    </div>
  </div>
</template>

<script>
import HomeCountdownCard from '@/components/HomeCountdownCard'
export default {
  name: 'HomeUpcomingEvents',
  data () {
    return {}
  },
  components: { HomeCountdownCard },
  methods: {
    handleScrollLeft () {
      if (window.matchMedia('screen and (max-width: 640px)').matches) {
        // eslint-disable-next-line no-unused-expressions
        this.$refs.scrollerCards ? this.$refs.scrollerCards.scrollLeft -= 150 : 0
      } else if (window.matchMedia('screen and (max-width: 768px)').matches) {
        // eslint-disable-next-line no-unused-expressions
        this.$refs.scrollerCards ? this.$refs.scrollerCards.scrollLeft -= 250 : 0
      } else {
        // eslint-disable-next-line no-unused-expressions
        this.$refs.scrollerCards ? this.$refs.scrollerCards.scrollLeft -= 450 : 0
      }
    },
    handleScrollRight () {
      if (window.matchMedia('screen and (max-width: 640px)').matches) {
        // eslint-disable-next-line no-unused-expressions
        this.$refs.scrollerCards ? this.$refs.scrollerCards.scrollLeft += 150 : 0
      } else if (window.matchMedia('screen and (max-width: 768px)').matches) {
        // eslint-disable-next-line no-unused-expressions
        this.$refs.scrollerCards ? this.$refs.scrollerCards.scrollLeft += 250 : 0
      } else {
        // eslint-disable-next-line no-unused-expressions
        this.$refs.scrollerCards ? this.$refs.scrollerCards.scrollLeft += 450 : 0
      }
    }
  }
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
