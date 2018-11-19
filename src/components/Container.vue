<template>
  <div class="hello">
    <MyButton />
    <BaseButton />
    <Hello title="42"/>
    <MySlot>
    </MySlot>
  </div>
</template>

<script>
import MyButton from "./MyButton";
import Hello from './Hello';
import MySlot from './Slot';
export default {
  name: 'Container',
  components: {
    MyButton,
    Hello,
    MySlot,
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
.hello{
  font-size: 24px;
  border: 1px solid red;
}
</style>
