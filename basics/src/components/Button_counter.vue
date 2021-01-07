<template>
    <div>
        <button v-on:click="count++">You clicked me {{ count }} times.</button>
    </div>
</template>

<script>
    export default {
        name: "button_counter",
        data: function () {
            return {
            count: 0
            }
        },
    };
</script>

<style></style>