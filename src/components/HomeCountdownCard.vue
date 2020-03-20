<template>
  <div class="w-full shadow-2xl">
    <div class="flex">
      <div class="">
        <img alt="children-sitting" src="../../images/children-sitting.png" style="height: 100%; width: 100%; object-fit: fill"/>
      </div>
      <div class="flex w-11/12">
        <div class="w-11/12 mx-12 my-8">
          <h3>Ikoyi Orphanage</h3>
          <span>Campaign description goes here</span>
          <br/>
          <hr style="margin-top: 30px; margin-bottom: 30px" >
          <div class="flex items-center" style="margin-bottom: 22px">
            <p class="my-auto" style="width: 6px; height: 6px; margin-right: 10px"><img alt="ellipse" src="../../images/ellipse.svg"></p>
            <p class="my-auto date">July 20, 2020</p>
          </div>
          <div class="flex">
            <div class="time-wrapper">
              <span class="time day-color">1</span>
              <span class="time day-color">8</span>
              <p class="day-word">Days</p>
            </div>
            <div class="time-wrapper">
              <span class="time time-color">2</span>
              <span class="time time-color">0</span>
              <p class="day-word">Hours</p>
            </div>
            <div class="time-wrapper">
              <span class="time time-color">2</span>
              <span class="time time-color">0</span>
              <p class="day-word">Minutes</p>
            </div>
          </div>
          <br/>
          <hr style="margin-top: 30px; margin-bottom: 30px" >
          <div id="fund-btn" class="flex items-center justify-center cursor-pointer">
            Fund Campaign
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeCountdownCard'
}
</script>

<style scoped>
  h3 {
    font-family: Cera Pro,serif;
    font-style: normal;
    font-weight: 900;
    font-size: 20px;
    line-height: 25px;
    color: #141414;
    margin-bottom: 10px;
  }
  span {
    font-family: Cera Pro, serif;
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 20px;
    color: #565050;
    margin-bottom: 30px;
  }
  hr {
    display: block;
    margin: 0.5em auto;
    border-style: inset;
    border-width: 1px;
    border-color: #F18500;
  }
  .date {
    font-family: Cera Pro, serif;
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    line-height: 23px;
    color: #141414;
  }
  .time {
    width: 36px;
    height: 42px;
    background-color: #F8FAFA;
    border-radius: 2px;
    font-family: Arial,serif;
    font-style: normal;
    font-weight: normal;
    font-size: 28px;
    line-height: 42px;
    vertical-align: middle;
    display: inline-block;
    text-align: center;
    margin-right: 2px;
    margin-top: auto;
    margin-bottom: auto;
  }
  .day-color {
    color: #000000;
  }
  .time-color {
    color: #999999;
  }
  .time-wrapper {
    margin-right: 20px;
  }
  .day-word {
    font-family: Cera Pro,serif;
    font-style: normal;
    font-weight: 300;
    font-size: 14px;
    line-height: 18px;
    color: #000000;
    text-align: center;
    margin-top: 10px;
  }
  #fund-btn {
    max-width: 190px;
    height: 42px;
    color: #FFFFFF;
    font-family: Cera Pro, serif;
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 20px;
    background-color: #F18500;
    border-radius: 3px;
  }
</style>
