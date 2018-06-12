<template>
  <div id="roomates">
    <ul>
      <li v-for="roomate in roomates" v-on:click="roomate.show = !roomate.show">
      <h2>{{ roomate.name }}</h2>
      <h3 v-show="roomate.show">{{ roomate.speciality }}</h3>
      </li>
    </ul>
  </div>
</template>

<script>

export default {
  data () {
    return {
      roomates: [
               {name: 'Ryu', speciality: 'Vue Components', show: false},
               {name: 'Crystal', speciality: 'HTML Wizardry', show: false},
               {name: 'Hitoshi', speciality: 'Click Events', show: false},
               {name: 'Tango', speciality: 'Conditionals', show: false},
               {name: 'Kami', speciality: 'Webpack', show: false},
               {name: 'Yoshi', speciality: 'Data Diggin', show: false}
      ]
    }
  },
}//end of export

</script>

<style scoped>
#roomates{
    width: 100%;
    max-width: 1200px;
    margin: 40px auto;
    padding: 0 20px;
    box-sizing: border-box;
}
ul{
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;
}
li{
    flex-grow: 1;
    flex-basis: 300px;
    text-align: center;
    padding: 30px;
    border: 1px solid #222;
    margin: 10px;
}
</style>
