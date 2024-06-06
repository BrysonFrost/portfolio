<script setup>
    const{ path } = useRoute();

    const { data } = await useAsyncData(`content-${path}`, () => {
        return queryContent()
        .where({_path: path})
        .findOne()
    })
</script>

<template>
    <ContentRenderer :value="data" class="container"/>
    <div class="container vh-100">
        <p>Tags:</p>
        <a v-for="tag in data.tags " :key="tag" :href="'/blog/tags/${tag}'" class="btn btn-primary">
            <Icon name="mdi:tag" size="1.5rem" color="white" /> {{ tag }}
        </a>
    </div>
</template>