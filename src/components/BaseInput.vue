<template>
    <input v-model="text" @keyup="this.change"/>
</template>

<script>
export default {
  name: 'BaseInput',
  data () {
    return {
counter:0,
      text: '',
    }
  },
  methods: {
    change: function(e){
        console.log(e.target.value)
        this.$emit('inputChage', e.target.value)

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
