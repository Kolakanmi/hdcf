<template>
  <div class="p-2" style="height: 100%; width: 100%; position: relative">
    <div class="" style="height: 100%; width: 100%; position: relative;">
      <div class="children-front">
        <img alt="children-front" src="../../images/children-front.png" style="height: 100%; width: 100%; object-fit: fill"/>
      </div>
      <div class="children-back">
        <img alt="children-back" src="../../images/children-back.png" style="height: 100%; width: 100%; object-fit: fill"/>
      </div>

    </div>
  </div>

</template>

<script>
export default {
  name: 'HomeDoubleImage'
}
</script>

<style scoped>
  .children-front {
    position: absolute;
    top: 30%;
    left: 0;
    display: block;
    width: 55%;
    height: 65%;
    padding: 6px;
    z-index: 10;
  }
  .children-front:after {
    content: "";
    position: absolute;
    top: 0;
    left: 50%;
    right: 0;
    bottom: 0;
    height: 100%;
    width: 50%;
    border-top: 6px solid #FFC37A;
    border-right: 6px solid #FFC37A;
    border-bottom: 6px solid #FFC37A;
  }
.children-back {
  position: absolute;
  left: 40%;
  top: 5%;
  display: block;
  width: 50%;
  height: 60%;
  padding: 6px;
}
.children-back:after {
  content: "";
  position: absolute;
  top: 0;
  left: 34%;
  right: 0;
  bottom: 0;
  height: 90%;
  width: 66%;
  border-top: 6px solid #FFC37A;
  border-right: 6px solid #FFC37A;
}

</style>
