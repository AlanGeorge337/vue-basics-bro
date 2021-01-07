<template>
    <div>
        <Child :greeting="greeting" :icecream="icecream" />
    </div>
</template>

<script>
    import Child from "../components/Child";
    import array_man from "../components/array_man";
    
    export default {
        data(){
            return {
                greeting: "Welcome to Props",
                icecream: ["Chocolate", "Vanilla", "Strawberry", "Pistachio"],
            };
        },
        components: {
            Child, array_man,
        },
    };

</script>
    
    
<style>

</style>