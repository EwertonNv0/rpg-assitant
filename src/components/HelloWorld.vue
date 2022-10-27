<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return{
      msg2: 'Fãs do DJ Gil Bala',
      contador: 0
    }
  },
  methods:{
    aumentaContador(){
      this.contador+=1000
    }
  }
}
</script>

<template>
  <p>{{ msg2 }}</p>
  <p>{{ contador }}</p>
  <button @click='aumentaContador'>Aqui carai</button>
</template>

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
