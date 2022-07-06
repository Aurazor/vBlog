<template>
  <div class="blog-items-wrapper">
  <div class="blog-items" v-for="(item,index) in items" :key="index">
      <BlogItem :item="item"/>
  </div>
  </div>
</template>

<script>
import BlogItem from "@/components/BlogItem";
export default {
  name: "RecentBlogs",
  props: {
    items: Array,
  },
  components:{
    BlogItem
  }
}
</script>

<style lang="scss" scoped>
  .blog-items{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-column-gap: 20px;
  }
</style>