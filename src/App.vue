<template>
  <div id="app">
    <NavSidebar :isSidebarOpen="isSidebarOpen" :setSidebarOpen="setSidebarOpen"/>
    <router-view :isSidebarOpen="isSidebarOpen" :setSidebarOpen="setSidebarOpen"></router-view>
  </div>
</template>

<script>
import NavSidebar from '@/components/NavSidebar'
export default {
  components: { NavSidebar },
  data () {
    return {
      isSidebarOpen: true
    }
  },
  methods: {
    setSidebarOpen (value) {
      this.isSidebarOpen = value
    }
  }
}
</script>

<style lang="scss">
  #app {
    position: relative;
  }
  .no-scroll-overlay {
    height: 99.9vh !important;
    overflow-y: hidden !important;
    opacity: 0.5;
  }

</style>
