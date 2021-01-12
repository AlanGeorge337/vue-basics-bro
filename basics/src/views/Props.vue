<template>
    <div>
        <Child :greeting="greeting" :icecream="icecream" />
        <array_man> </array_man>

        <div id="app">{{ info }}</div>

    </div>

</template>

<script>
    import Child from "../components/Child";
    import cheap_shark from "../components/cheap_shark";
    
    export default {
        // data(){
        //     return {
        //         greeting: "Welcome to Props",
        //         icecream: ["Chocolate", "Vanilla", "Strawberry", "Pistachio"],
        //     };
        // },
        
        components: {
            Child, cheap_shark,
        },

        name: "maps",
        data () {
            return {
            info: null
            }
        },
        mounted () {
            axios
            .get('https://countriesnow.space/api/v0.1/countries/flag/images')
            .then(response => (this.info = response))
  }
    };

</script>
    
    
<style>

</style>