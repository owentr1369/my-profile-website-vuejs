<template>
  <div class="blog-card-wrap">
    <div class="container">
      <h3>View More Recent Blogs</h3>
      <div class="blog-cards">
        <ProjectsCard
          :post="post"
          v-for="(post, index) in sampleBlogCards"
          :key="index"
        />
      </div>
    </div>
  </div>
</template>

<script>
import ProjectsCard from "../components/ProjectsCard.vue";
export default {
  components: {
    ProjectsCard,
  },
  computed: {
    sampleBlogCards() {
      return this.$store.state.sampleBlogCards;
    },
  },
};
</script>

<style lang="scss" scoped>
h1 {
  color: #000;
}
</style>