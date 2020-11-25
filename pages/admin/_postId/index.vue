<template>
    <div class="admin-post-form">
        <section class="update-form">
            <AdminPostForm :post="loadedPost" />
        </section>
    </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'
export default {
    layout: 'admin',
    components: {
        AdminPostForm
    },
    data() {
        return {
            loadedPost: {
                author: 'Mobarak Hossain',
                title: 'My awesome post',
                content: 'Super amazing, thanks for that!',
                thumbnailLink: 'https://www.thefinancialexpress.com.bd/uploads/1544961142.jpg'
            }
        }
    }
}
</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>
