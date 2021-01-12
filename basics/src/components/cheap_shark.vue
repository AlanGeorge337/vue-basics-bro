<template>
    <div>
        <ul id="cheap_shark">
            <li v-for="item in items" :key="item.message">
            {{ item.message }}
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: "cheap-shark",
        
    
       
       
       
       
       // name: "array_man",
        // data() {
        //     return{
        //         items: [
        //         { message: 'Apple' },
        //         { message: 'Banana' },
        //         { message: 'Strawberry' },
        //         { message: 'Orange' },
        //         { message: 'Watermelon' },
        //         { message: 'Grape' },
        //     ]
        //     }
        // } 
    };
</script>

<style></style>