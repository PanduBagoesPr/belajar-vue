<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <div>Saya adalah {{ name }}</div>
    <div>Tahun ini umur saya : {{ umur + 1 }}</div>
    <ButtonCounter/>
    
  </div>
</template>

<script>
import ButtonCounter from './ButtonCounter.vue'

export default {
  name: 'HelloWorld',
  components: {
    ButtonCounter
  },
  props: {
    msg: String
  },
  data: function () {
    return {
      name : "Pandu",
      umur : 19,
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
