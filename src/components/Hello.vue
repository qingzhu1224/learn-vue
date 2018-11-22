<template>
  <div class="hello">
    我是hello
    <MyInput
      @listenerChildChange="this.inputChange"
    />
    <div>{{ title }}</div>
    <MySlot>
      <h1>我是个好孩纸</h1>
    </MySlot>
  </div>
</template>

<script>
import MyInput from './MyInput';
import MySlot from './Slot';
export default {
  name: 'Hello',
  components: {
    MyInput,
    MySlot,
  },
  props: {
    title: String,
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
      inputChange: function(data){
        console.log(`我是子組件傳遞過來的${data}`)
      }
  }
}
</script>
