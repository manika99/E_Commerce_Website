<template>
<div>
  <app-header></app-header>
  <section-women v-bind:items="items"></section-women>
  <hr>
  <section-men v-bind:items="items"></section-men>
  <app-footer></app-footer>
</div>
</template>

<script>
import Header from './Components/Header.vue';
import Footer from './Components/Footer.vue';
import Women from './Components/Women.vue';
import Men from './Components/Men.vue';
export default {
  components:{
    'app-header': Header,
    'app-footer': Footer,
    'section-women': Women,
    'section-men': Men
  },
  data () {
    return {
      items: [
                { name: 'Indian Wear', speciality: 'Fresh arrival || Sale', show: false },
                { name: 'Western Wear', speciality: 'Fresh arrival || Sale', show: false },
                { name: 'Accessories', speciality: 'Fresh arrival || Sale', show: false },
                { name: 'Footwear', speciality: 'Fresh arrival || Sale', show: false },
                { name: 'Handbags', speciality: 'Fresh arrival || Sale', show: false },
                { name: 'Skincare', speciality: 'Fresh arrival || Sale', show: false }
            ]
    }
  }
}
</script>

<style>
body{
  background: rgb(183, 183, 248);
  margin: 0;
}


</style>
