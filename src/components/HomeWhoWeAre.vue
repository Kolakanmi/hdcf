<template>
  <div class="md:flex">
    <div class="md:w-4/12" style="">
      <img alt="children" src="../../images/home-section3.png" style="height: 100%; width: 100%; object-fit: fill"/>
    </div>
    <div id="who-we-are" class="flex items-center justify-center md:w-8/12">
      <div class="w-3/4">
        <h3>Who Are We</h3>
        <p>
          It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.
          The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here
          , content here'.
        </p>
        <p>
          It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.
          The point of using.
        </p>
        <div id="readmore-btn" class="flex items-center justify-center cursor-pointer">
          Read More
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeWhoWeAre'
}
</script>

<style scoped>
#who-we-are {
  background-color: #FFF7ED;
}
h3 {
  font-family: Cera Pro,serif;
  font-style: normal;
  font-weight: 900;
  font-size: 28px;
  line-height: 35px;
  color: #141414;
  margin-bottom: 30px;
}
p {
  font-family: Cera Pro, serif;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 160%;
  color: #000000;
  margin-bottom: 20px;
}
#readmore-btn {
  max-width: 152px;
  height: 52px;
  color: #F18500;
  font-family: Cera Pro, serif;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 20px;
  border: 2px solid #F18500;
  border-radius: 3px;
}
</style>
