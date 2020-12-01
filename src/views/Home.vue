<template>
  <div class="container">
    <div>
        <b-card class="mt-4" v-for="post in posts" :key="post.title" :title="post.title" header-tag="header" footer-tag="footer">
          <b-card-text>{{ post.description }} #{{ post.id + 1 }}</b-card-text>
          <b-button href="#" variant="primary">Go somewhere</b-button>
        </b-card>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home.vue',
  data () {
    return {
      posts: [
        { id: 0, title: 'Post 1', description: 'Описание поста' },
        { id: 1, title: 'Post 2', description: 'Описание поста' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
