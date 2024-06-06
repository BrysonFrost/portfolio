<script setup>
const { data: posts } = await useAsyncData('posts', () =>
    queryContent('/blog').find()
)
</script>

<template>

    <h1>These are my blog posts</h1>
    <ul>
        <li v-for="post in posts" :key="post._id">
            <nuxt-link :to="post._path" class="text-primary">{{ post.title }}</nuxt-link>
            <p>{{ post.description }}</p>
        </li>
    </ul>


</template>