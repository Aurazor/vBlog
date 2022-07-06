<template>
  <div class="blog-item">
    <div class="blog-img">
      <img v-bind:src="item.img" alt="#">
    </div>
    <div class="blog-tags">
        <div class="blog-tag"  v-for="(tag,index) in item.tags" :key="index">
          {{ tag }}
        </div>
    </div>
    <div class="blog-title">
<!--      Creating is a privilege but it’s also a gift-->
      {{ item.title }}
    </div>
    <div class="blog-desc">
      {{ item.desc }}

      <!--      Nullam vel lectus vel velit pellentesque dignissim nec id magna. Cras molestie ornare quam at semper. Proin a ipsum ex...-->
    </div>
  </div>
</template>

<script>
export default {
  name: "BlogItem",
  props: {
    item: Object,
  },
}
</script>

<style lang="scss" scoped>
  .blog-item{
    .blog-img{
      img {
        width: 100%;
        border-radius: 20px;
      }
    }
    .blog-tags{
      margin: 10px 0;
      .blog-tag{
        font-size: 13px;
        border-radius: 20px;
        display: inline-block;
        padding: 5px 8px;
        background-color: #efeef0;
        margin-right: 5px;
      }
    }

    .blog-title{
      font-size: 20px;
      font-weight: bold;
      color: #151618;
      margin-bottom: 10px;
    }
  }
</style>