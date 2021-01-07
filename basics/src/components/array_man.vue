<template>
    <div>
        <ul id="array_man">
            <li v-for="item in items" :key="item.message">
            {{ item.message }}
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: "array_man",
        data() {
            return{
                items: [
                { message: 'Apple' },
                { message: 'Banana' },
                { message: 'Strawberry' },
                { message: 'Orange' },
                { message: 'Watermelon' },
                { message: 'Grape' },
            ]
            }
        } 
    };
</script>

<style></style>