<template>
  <div class="my-btn">
    <button v-on:click="handleClick">Добавить</button>
  </div>
</template>

<script>
export default {
  name: "MyButton",
  methods: {
    handleClick() {
      this.$emit("button-click"); 
    },
  },
};
</script>
  
  <style>
  .my-btn {
    position: absolute;
    top: 40px;
    right: 500px;
    width: 100px;
    height: 40px;
    background-color: rgb(123, 159, 206, 0.214);
    border-radius: 10px;
  }
  
  .my-btn button {
    font-size: 16px;
    width: 100%;
    height: 100%;
    background: none;
    cursor: pointer;
    border: none;
  }
  </style>
  