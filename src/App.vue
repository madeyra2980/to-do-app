  <template>
    <div class="app">
      <div class="top-item">
        <MyInput @input-value-changed="handleInputValueChanged" />
        <MyButton @button-click="handleButtonClick" />
      </div>
      <ListItem :listData="listData" />
    </div>
  </template>

  <script>
  import MyInput from "./components/MyInput.vue";
  import ListItem from "./components/ListItem.vue";
  import MyButton from "./components/MyButton.vue";

  export default {
    name: "App",
    components: {
      MyInput,
      MyButton,
      ListItem,
    },
    data() {
      return {
        inputValue: "",
        listData: [],
      };
    },
    methods: {
      handleInputValueChanged(value) {
        this.inputValue = value;
      },
      
      handleButtonClick() {
        this.listData.push({ id: this.listData.length + 1, body: this.inputValue });
        this.inputValue = "";
      },  
    }
  }
      
  </script>

  <style>
  * {
    padding: 0;
    margin: 0;
  }

  .top-item {
    width: 100%;
    background-color: aqua;
    display: flex;
    background: none;
    height: 200px;
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
    width: 100%;
    background-color: rgb(200, 210, 217);
  }
  </style>
