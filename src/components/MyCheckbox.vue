<template>
    <input v-model="text" @change="this.keyupEvent"/>
</template>

<script>
export default {
  name: 'MyCheckbox',
  data () {
    return {
      counter:0,
      text: '',
    }
  },
  methods: {
    keyupEvent: function(e){
      const { value } = e.target;
      console.log(value);
      this.$emit('listenerChildChange', value);
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
