<template>
  <div class="my-input">
    <input tabindex="6" type="text" v-model="inputValue" placeholder="Введите задачу">
  </div>
</template>
  
<script>
export default {
  name: 'MyInput',
  data() {
    return {
      inputValue: ''
    };
  }
}
</script>
  
<style>
.my-input {
  opacity: .7;
  background-color: rgb(133, 190, 203);
  width: 400px;
  height: 40px;
  text-align: center;
  border-radius: 10px;
}

.my-input input {
  text-align: center;
  width: 100%;
  border: none;
  height: 100%;
  font-size: 20px;

  background: none;
}
</style>
  