<template>
  <div class="hello">
    <h1>{{ msg }} {{ any }}</h1>
    <p v-bind:class="valorClasse">{{description}}</p>
    <ul>
      <li v-for="(n, i) in nombres" v-bind:n="n" v-bind:key="n.id">{{i}} = {{n}}</li>
    </ul>
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String, 
    any: Number
  },
  data: function() {
    return {
      description: "I am a Vue CLI Component",
      valorClasse: "estil",
      nombres: [
        "Maria", "Pep", "Lluis"
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  background-color: aqua;
}

.estil {
  color:blue;
  font-size: 2.5em;
  font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}


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
