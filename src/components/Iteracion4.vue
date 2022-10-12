<template>
    <div v-for="elem in data">
        {{elem.title}}
        {{elem.content}}
    </div>
</template>
<script setup>
import { ref } from 'vue';

const data = ref([
    {
        title: 'dog',
        description: 'brown',
        content: 'sjkdbnkjsvjkev'

    }, {
        title: 'cat',
        description: 'gray',
        content: 'skjvkjdrv'
    },
    {
        title: 'fish',
        description: 'orange',
        content: 'kjh'
    }])
</script>
<style scoped>

</style>