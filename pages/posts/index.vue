<template>
    <div class="posts-page">
        <PostList />
    </div>
</template>

<script>
import PostList from '@/components/Posts/PostList'
export default {
    components: {
        PostList
    }
}
</script>

<style scoped>
.posts-page{
    display: flex;
    text-align: center;
    justify-content: center;
}
</style>
