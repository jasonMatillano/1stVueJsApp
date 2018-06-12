<template>
  <div>
    <app-header></app-header>
    <app-roomates></app-roomates>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './Header.vue';//import (object_name) from (file_name);
import Footer from './Footer.vue';//import (object_name) from (file_name);
import Roomates from './Roomates.vue';//import (object_name) from (file_name);

export default {
  components: {
    'app-header': Header, //'conponent_name': (object_name)
    'app-footer': Footer, //'conponent_name': (object_name)
    'app-roomates': Roomates, //'conponent_name': (object_name)
    
  },

  data () {
    return {
    }
  },
}//end of export

</script>

<style>
</style>
