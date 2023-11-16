<template>
  <div class="Lists" v-for="item in listData" :key="item.id">
    <ul>
      <li>{{ item.body }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    listData: {
      type: Array,
      default: () => [{ id: 1, body: "Сделать задачку" }]
    }
  },
  name: 'ListItem'
}
</script>

<style>
.Lists {
  margin-top: 40px;
  background-color: #67625c;
  width: 500px;
  font-size: 24px;
}
</style>
