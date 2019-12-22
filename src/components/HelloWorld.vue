<template>
  <div class="hello">
    <h6>{{ msg }}</h6>
    <p>
    </p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .hello{
    left: 1rem;
    margin: 0.2rem;
  }
h3 {
  margin: 10px 0 0;
  top: 20px;
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
