<template>
  <div class="blog-items-wrapper">
    <p class="blog-items-heading">See what we've <br> <span> written lately</span></p>
    <div class="blog-items">
      <BlogItem :item="item" v-for="(item,index) in items" :key="index"/>
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

.blog-items-wrapper{
  margin: 30px 0;
  padding: 30px 0;
  border-top: 1px solid #e0e0e0;
  .blog-items-heading{
    font-size: 51px;
    margin-bottom: 10px;
    span{
      font-weight: bold;
      background: linear-gradient(to bottom left, #94F568, #2959A7);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
  }
  .blog-items{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-column-gap: 20px;
    grid-row-gap: 20px;
  }
}

</style>