<script setup>
import { ref } from 'vue';
import PostCard from './components/PostCard.vue';

const data = ref([])
fetch('https://jsonplaceholder.typicode.com/posts')
    .then((resp) => resp.json())
    .then((d) => data.value = d)
    .finally(() => console.log('End api'))

</script>

<template>
    <h5 class="display-5 text-primary">Home Page of Post</h5>
    <button class="btn btn-primary me-3">Back</button>
    <button class="btn btn-primary">Next</button>
    <hr>

    <PostCard v-for="p in data" :key="p.id" :id="p.id" :title="p.title" :body="p.body">
    </PostCard>
</template>
