<template>
  <div class="hello">
    <MyButton />
    <BaseButton />
    <Hello title="42"/>
  </div>
</template>

<script>
import MyButton from "./MyButton";
import Hello from './Hello';
export default {
  name: 'Container',
  components: {
    MyButton,
    Hello,
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
