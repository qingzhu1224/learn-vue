<template>
  <div class="hello">
    我是hello
    <MyInput
      @listenerChildChange="this.inputChange"
    />
    <div>{{ title }}</div>
  </div>
</template>

<script>
import MyInput from './MyInput';
export default {
  name: 'Hello',
  components: {
    MyInput,
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
