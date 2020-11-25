<template>
    <section class="post-list">
        <PostPreview
            id="1"
            :is-admin = "isAdmin"
            thumbnail="https://www.thefinancialexpress.com.bd/uploads/1544961142.jpg"
            title="Hello There!"
            previewText="This is my first post"
        />
        <PostPreview
            id="2"
            :is-admin = "isAdmin"
            thumbnail="https://static.wixstatic.com/media/b6a0a6_431d6337ed6d43a1b8a91d82a8cb7a1f~mv2.jpg"
            title="Hello There - the secount time!"
            previewText="This is my secound post"
        />
        <PostPreview
            id="3"
            :is-admin = "isAdmin"
            thumbnail="https://image.freepik.com/free-photo/businessman-using-tech-devices-icons-thin-line-interface_117023-904.jpg"
            title="Hi!"
            previewText="This is my third post"
        />
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
    components: {
        PostPreview
    },
    props: {
        isAdmin: {
            type: Boolean,
            default: false
        }
    }
}
</script>

<style scoped>
.post-list {
    display: flex;
    padding: 20px;
    box-sizing: border-box;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
}
</style>
