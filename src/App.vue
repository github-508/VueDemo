<template>
 <div>
  <!--img alt="Vue logo" src="./assets/logo.png"-->
  <!--HelloWorld msg="Welcome to Your Vue.js App"/-->
  <!--Test></Test-->
    <div>
      {{msg}}
    </div>
    <div>
      {{msg1}}
    </div>
    <div>
      {{msg2}}
    </div>
    <button @click="add">
      确认
    </button>
    <div>
      {{ans}}
    </div>
 </div>
</template>

<script>

//import Test from './components/test'

export default {
  name: 'App',
  data() {
    return {
      msg: "var1",
      msg1:"var2",
      msg2:"var3",
      ans:0,
      a:1,
      b:2,

    }
  },
  methods: {
    add() {
      var aa = 10;
      var bb = 11;
      this.a = 10;
      this.b = 15;
      this.ans = this.a+ this.b + aa + bb;
      this.a = 1;
      this.b = 8;
      this.ans = 10;
      aa = 12;
      bb = 13;
      this.ans = this.a * this.b + aa + bb;
    }
  },
  components: {
    //Test
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
