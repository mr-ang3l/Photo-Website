<script setup>
import {ref} from 'vue'


</script>

<template>
    <section id="navigator">
        <a href="" target="_blank">Home</a>
        <a href="" target="_blank">About</a>
        <a href="" target="_blank">Contact</a>
        <a href="" target="_blank">Work</a>
    </section>
</template>

<style scoped>
    #navigator {
        margin-block: 10px;
        display: flex;
        flex-direction: row nowrap;
        justify-content: space-around;
        align-items: center;
        background: rgba(255, 255, 255, 0.87);
    }

    a {
        font-weight: bold;
        color: #003049;
        font-size: 1em;
    }
</style>