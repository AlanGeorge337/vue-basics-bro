<template>
    <div>
        <!-- <Child :greeting="greeting" :icecream="icecream" />
        <array_man> </array_man> -->

        <!-- <div id="app">{{ info }}</div> -->
        <div>Maps and Info</div>
        <table border="1rem">
            <tr>
                <td>Flag</td>
                <td>Name</td>
            </tr>
            <tr v-for="item in list" v-bind:key="item.id">
                <td>{{item.name}}</td>
                <td>{{item.flag}}</td>
            </tr>
        </table>

        <maps_and_info />

    </div>
  
</template>

<script>
    // import Child from "../components/Child";
    import maps_and_info from "../components/maps_and_info";
    import axios from 'axios';
    
    export default {
        // data(){
        //     return {
        //         greeting: "Welcome to Props",
        //         icecream: ["Chocolate", "Vanilla", "Strawberry", "Pistachio"],
        //     };
        // },
        
        components: {
            // Child,
            maps_and_info,
        },
        name: "maps",
        data () {
            return {
            list: undefined
            }
        },
        mounted () {
            axios
            .get('https://countriesnow.space/api/v0.1/countries/flag/images')
            .then(response => {
                this.list = response.data.data;
                this.info = response.data.data;
            })
        }
    };

</script>
    
    
<style>

</style>