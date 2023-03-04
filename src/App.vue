<template>
<div>
  <app-header></app-header>
  <app-items></app-items>
  <hr>
  <app-footer></app-footer>
</div>
</template>

<script>
import Header from './Components/Header.vue';
import Footer from './Components/Footer.vue';
import Items from './Components/Items.vue'
export default {
  components:{
    'app-header': Header,
    'app-footer': Footer,
    'app-items': Items
  },
  data () {
    return {
    
    }
  }
}
</script>

<style scoped>

</style>
