<template>
  <div class="my-input">
    <input
    v-model="inputValue"
    @input="inputValueTarget" 
    tabindex="6" 
    type="text"  
    placeholder="Введите задачу"/>
  </div>
</template>

<script>
export default {
  name: 'MyInput',
  components:{
  },
  data() {
    return {
      inputValue: " "
    };
  },
  methods:{
    inputValueTarget(){
      this.$emit('input-value-changed', this.inputValue);
    }
  }
}
</script>

<style>
.my-input {
  background-color: rgb(168, 217, 228);
  opacity: .6;
  width: 100%;
  height: 120px;
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
  height: 50px;
}
</style>
