<template>
  <div class="about">
    <NavHeader/>
    <h1>This is an about page</h1>
  </div>
</template>

<style>
  .about {
    padding: 20px;
    background-color: white;
  }
</style>
<script>
import NavHeader from '@/components/NavHeader'
export default {
  components: { NavHeader }
}
</script>
