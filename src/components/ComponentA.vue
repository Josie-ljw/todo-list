<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <button v-on:click="onClickMe">Click！</button>
    <button v-on:click="onClickMe">open mouse!</button>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      msg: 'hello from component a!'
    }
  },
  props: ['msgfromfather'],
  methods: {
    onClickMe: function () {
      console.log(this.msgfromfather);
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
