<template>
  <div class="app">
    <TopItem/>
    
  </div>
</template>

<script>
import TopItem from './components/TopItem.vue'
export default {
  name: 'App',
  components: {
   TopItem

  }
}
</script>

<style>
* {
  background-color: rgb(88, 70, 70);
  padding: 0;
  margin: 0;
}

.app {
  background: url("/src/assets/images/auth_background.jpg") no-repeat;
  background-size: cover;
  height: 100vh;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 auto;
  background: url("/src/assets/images/auth_background.jpg") no-repeat cover;
  background-color: rgb(200, 210, 217);
}

</style>
