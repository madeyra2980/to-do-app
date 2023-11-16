<template>
    <div class="top-item">
        <MyInput />
        <MyButton />
    </div>
</template>


<script>
import MyButton from './MyButton.vue';
import MyInput from './MyInput.vue';
export default {
    name: 'TopItem',
    components: {
        MyInput,
        MyButton,

    }
}
</script>

<style>

.top-item {
  display: flex;
  height: 60px;
  align-items: center;
  margin-top: 60px;
  background: none;
  gap: 20px;

}
</style>