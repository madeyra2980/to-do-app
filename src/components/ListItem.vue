<template>
  <div class="rod">
  <div class="Lists" v-for="item in listData" :key="item.id">
    <ul>
      <li>{{ item.body }}</li>
    </ul>
  </div>
</div>
</template>

<script>
export default {
  props: {
    listData: {
      type: Array,
      default: () => [{ id: 1, body: "" }]
    }
  },
  name: 'ListItem'
}
</script>

<style>

.Lists {
  margin-top: 40px;
  width: 500px;
  font-size: 24px;
  height: 100vh;
  overflow: auto;
  box-sizing: border-box; 

}



.Lists ul li{
  width: 300px;
  list-style-type: none;
  padding: 20px;
  font-size: 30px;
  font-weight: bold;
  border: 1px solid rgb(139, 173, 180);
  color:  rgb(100, 135, 143);
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
</style>
