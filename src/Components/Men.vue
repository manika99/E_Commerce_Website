<template>
    <div id="items">
        <h2>{{category}}</h2>
        <ul>
            <li v-for="item in items" v-bind:key="item.name" v-on:click="item.show = !item.show">
                <h2>{{item.name}}</h2>
                <h3 v-show="item.show">{{item.speciality}}</h3>
            </li>
        </ul>
    </div>
</template>
    
<script>
export default {
    props: ['items'],
    data() {
        return {
           category:'Men'

        }
    }
}
</script>
    
<style scoped>
#items{
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
h2 {
    color: #222;
    text-align: center;
  }
</style>