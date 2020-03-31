<template>
  <div class="home">
    <div id="first-page" class="">
      <div style="height: 15vh">
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
    <div id="email-footer" class="flex justify-center items-center m-auto h-full">
      <HomeEmailSubscribe/>
    </div>
    <div id="contact-us">
      <div class="w-1/3 text-center mx-auto">
        <h3>Contact Us</h3>
        <span>drop a message to get more info about our activities, we will love to hear from you.</span>
      </div>
      <div class="w-2/3">
        <form>
          <div class="w-1/2">
            <label>Name</label>
            <input>
          </div>
        </form>
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
    height: 300px;
    background-size: 100% 300px;
  }
  #contact-us {
    background-color: #FFF7ED;
  }
</style>
