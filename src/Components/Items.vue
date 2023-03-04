<template>
    <div id="items">
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
    data() {
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
</style>