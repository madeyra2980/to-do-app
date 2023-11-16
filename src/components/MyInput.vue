<template>
  <div class="my-input">
    <input tabindex="6" type="text"  placeholder="Введите задачу">
    <MyButton/>
  </div>
</template>

<script>
import MyButton from './MyButton.vue';
export default {
  name: 'MyInput',
  components:{
    MyButton
  },
  data() {
    return {
      inputValue: ''
    };
  },
  
}
</script>

<style>
.my-input {
  background-color: rgb(168, 217, 228);
  opacity: .6;
  width: 100%;
  height: 200px;
  text-align: center;
  border-radius: 10px;
  align-items: center;
  display: flex;
  justify-content: center;
  gap: 10px;
}

.my-input input {
  text-align: center;
  border: none;
  font-size: 20px;
  margin-left: 40%;
  height: 100px;
}
</style>
