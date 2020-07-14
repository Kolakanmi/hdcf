<template>
  <div class="home">
    <div id="first-page" class="">
      <div style="height: 10vh; margin-bottom: 5vh">
        <NavHeader/>
      </div>
      <div class="flex" style="height: 80vh;">
        <div class="flex md:w-1/2 my-auto items-center justify-center">
          <HomeFirstPageText/>
        </div>
        <div id="page-image" class="hidden md:flex w-1/2 mr-auto">
          <HomeDoubleImage/>
        </div>
      </div>
    </div>
    <div id="second-page" class="py-24">
      <div >
        <HomeMissionWrapper/>
      </div>
    </div>
    <div id="third-page">
      <HomeWhoWeAre/>
    </div>
    <div id="fourth-page">
      <HomeUpcomingEvents/>
    </div>
    <div id="email-footer" class="flex justify-center items-center h-full">
      <HomeEmailSubscribe/>
    </div>
    <div class="px-1" id="contact-us">
      <div class="w-full md:w-1/3 text-center mx-auto">
        <h3>Contact Us</h3>
        <span>Drop a message to get more info about our activities, we will love to hear from you.</span>
      </div>
      <div class="w-full md:w-2/3 mx-auto">
        <form class="my-8">
          <div class="block md:flex justify-center mx-auto">
            <div class="w-full md:w-1/2 md:mr-8 input-border">
              <label class="form-label" for="name">Name</label>
              <input id="name" class="appearance-none bg-transparent border-none w-full text-gray-700 py-1 leading-tight focus:outline-none" type="text">
            </div>
            <div class="w-full md:w-1/2 mt-8 md:mt-0 input-border ">
              <label class="form-label" for="email">Email</label>
              <input id="email" class="appearance-none bg-transparent border-none w-full text-gray-700 py-1 leading-tight focus:outline-none" type="email">
            </div>
          </div>
          <div class="input-border  mt-8">
            <label class="form-label" for="message">Message</label>
            <input id="message" class="appearance-none bg-transparent border-none w-full text-gray-700 py-1 leading-tight focus:outline-none" type="text">
          </div>
          <div class="flex justify-center mt-8">
            <button class="submit-button text-white font-bold py-2 px-4 rounded">Submit</button>
          </div>
        </form>
      </div>
    </div>
    <div id="home-footer" class="flex items-center justify-center" style="background-color: #F18500;height: 80px">
      <div class="flex">
        <img class="mr-2" src="../../images/copyright.svg" alt="copyright">
        <span class="text-white"> 2020. human development charity foundation</span>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import HomeDoubleImage from '@/components/HomeDoubleImage'
import NavHeader from '@/components/NavHeader'
import HomeFirstPageText from '@/components/HomeFirstPageText'
import HomeMissionWrapper from '@/components/HomeMissionWrapper'
import HomeWhoWeAre from '@/components/HomeWhoWeAre'
import HomeUpcomingEvents from '@/components/HomeUpcomingEvents'
import HomeEmailSubscribe from '@/components/HomeEmailSubscribe'
export default {
  name: 'Home',
  components: {
    HomeEmailSubscribe,
    HomeUpcomingEvents,
    HomeWhoWeAre,
    HomeMissionWrapper,
    HomeFirstPageText,
    NavHeader,
    HomeDoubleImage
  }
}
</script>

<style>
  #first-page {
    padding: 20px 8.33%;
    max-height: 100vh;
    background: url("../../images/background-gradient.png");
    background-size: 100% 100vh;
  }
  #page-image {
    position: relative;
    top: 0;
    padding: 0;
  }
  #second-page {
    padding-right: 14.5%;
    padding-left: 14.5%;
  }
  #fourth-page {
    padding-top: 150px;
    //padding-left: 13.68%;
    //margin-bottom: 150px;
  }
  #email-footer {
    margin-top: 150px;
    margin-bottom: 150px;
    background: url("../../images/background-footer-email.png");
    min-height: 300px;
    background-size: 100% 300px;
  }
  #contact-us {
    background-color: #FFF7ED;
    padding-top: 100px;
    padding-bottom: 100px;
  }
  #contact-us h3 {
    font-family: "Cera Pro",serif;
    font-style: normal;
    font-weight: 900;
    font-size: 28px;
    color: #141414;
  }

  #contact-us span {
    font-family: "Cera Pro", serif;
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    color: #565050;
  }
  .input-border {
    border-bottom: 1px solid #F18500;
  }

  form input {
    color: #141414 !important;
    font-family: "Cera Pro", serif;
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
  }

  .form-label {
    color: #565050;
  }

  .submit-button {
    background-color: #F18500;
  }
</style>
