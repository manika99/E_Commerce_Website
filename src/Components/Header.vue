<template>
  <div>
    <header>
      <h1>{{ title }}</h1>
    </header>
    <!-- <h1>{{ category }}</h1> -->
  </div>
</template>
  
<script>
export default {
  data() {
    return {
      title: 'Shoppers Destination',
      // category: 'Women'
    }
  }
}
</script>
  
<style scoped>
header {
  background: lavender;
  padding: 10px;

}

h1 {
  color: #222;
  text-align: center;
}
</style>