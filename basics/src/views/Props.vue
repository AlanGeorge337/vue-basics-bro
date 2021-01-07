<template>
    <div>
        <Child :greeting="greeting" :icecream="icecream" />
    </div>
</template>

<script>
    import Child from "../components/Child";
    import button_counter from "../components/Button_counter";
    
    export default {
        data(){
            return {
                greeting: "Welcome to Props",
                icecream: ["Chocolate", "Vanilla", "Strawberry", "Pistachio"],
            };
        },
        components: {
            Child, Button_counter,
        },
    };

</script>
    
    
<style>

</style>