<template>
    <div class="home">
        <BlogCard
                :key="post.id"
                v-for="post in posts"
                :id="post.id"
                :title="post.title"
                :date="post.date"
                :name="post.name"
                :description="post.description"
        />

    </div>
</template>

<script>
// @ is an alias to /src

import BlogCard from "@/components/BlogCard.vue";
import {postsData} from "@/assets/posts-data";

export default {
    name: 'HomeView',
    components: {
        BlogCard
    },
    data() {
        return {
            posts: postsData,
        }
    }
}

</script>

<style>
.home {
    max-width: 1200px;
    margin: 0 auto;
    width: 100%;
}
</style>
