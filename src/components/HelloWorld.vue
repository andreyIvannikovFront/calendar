<template>
  <div class="hello">
    {{date}}
    <vc-date-picker :maxDate="maxDate" :minDate="minDate" v-model="date" />
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      maxDate: new Date(2022, 11, 27),
      minDate: new Date(2022, 11, 16),
      date: new Date(),
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
