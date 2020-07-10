<template>
  <div>
    <h1>Las cosas que quiere comer {{ nombre }}: </h1>
    <ul>
      <li v-for="(lista,i) in listas" v-bind:key="i"> {{lista}}</li>
     </ul>
  </div>
</template>
<script>
export default {
  name: 'Lista',
  data:function(){
    return{
      nombre:'Odrita',
      listas:['Pizza','Sushi','Cazuela']                                        
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
  display: block;
  margin: 15px 10px;
  align-text:justify;
}
</style>
