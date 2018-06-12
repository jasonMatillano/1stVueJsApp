<template>
  <footer>
    <p>{{copyright}}</p>
  </footer>
</template>

<script>

export default {
  data () {
    return {
      copyright: '(C) Vue Roomates 2018'
    }
  },
}//end of export

</script>

<style scoped>
footer {
  background: #222;
  padding: 6px;
}
p {
  color: lightgreen;
  text-align: center;
}
</style>
