<template>
  <div class="home">
    <Login/>
  </div>
</template>

<script>
// @ is an alias to /src
import Login from '@/components/login.vue'

export default {
  name: 'Home',
  components: {
    Login
  }
}
</script>
<style>
.home{
  min-height: 100vh;
  display:flex;
  align-items: center;
  justify-content: center;
}
</style>
