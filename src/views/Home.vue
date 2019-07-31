<template>
  <div class="home">
    <img alt="project logo" src="../assets/logo-ktk.png">
    <home-description msg="Welcome to My App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeDescription from '@/components/home/HomeDescription.vue'

export default {
  name: 'home',
  components: {
    HomeDescription
  }
}
</script>

<style scoped>
    .home {
        text-align: center;
    }
</style>