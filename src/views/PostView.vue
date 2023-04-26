<template>
    <div v-if="post" class="post-page">
        <div class="post-title">
            {{ post.title }}
        </div>
        <div class="post-banner">
            <img :src="post.banner" alt="">
        </div>
        <div class="post-description">
            {{ post.description }}
        </div>
        <div class="post-meta">
            <div class="post-user">
                {{ post.name }}
            </div>
            <div class="post-date">
                {{ post.date }}
            </div>
        </div>


        <div class="post-text">
            {{ post.text }}
        </div>
    </div>
</template>

<script>
import {postsData} from "@/assets/posts-data";

export default {
    name: "PostView",
    data() {
        return {
            posts: postsData,
            post: null
        }
    },
    mounted() {
        this.post = this.posts.find(post => post.id === parseInt(this.$route.params.id))
    }
}
</script>

<style scoped>
.post-page {
    max-width: 600px;
    margin: 32px auto;
    width: 100%;
    padding-bottom: 60px;

}

.post-banner {
    display: block;
    border-radius: 20px;
    overflow: hidden;
}

.post-meta {
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 32px 0;
}

.post-user,
.post-date {
    font-size: 14px;

}

.post-user {
    color: #000;
}

.post-date {
    color: #a9a9a9;
    margin-left: 12px;
}

.post-title {
    font-size: 32px;
    color: #2c3e50;
    font-weight: 400;
    margin-bottom: 12px;
}

.post-description {
    font-size: 16px;
    line-height: 1.2;
    color: #bbbaba;
    margin: 6px 0;
    font-style: italic;
}

.post-banner img {
    width: 100%;
    height: auto;
    display: block;
}

.post-text {
    font-size: 20px;
    line-height: 1.5;
    color: #2c3e50;
    text-align: justify;
    margin: 32px 0;
}
</style>