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
      {{ item.title }}
    </div>
    <div class="blog-desc">
      {{ item.desc }}
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
        width:100%;
        height:380px;
        /*Scale down will take the necessary specified space that is 100px x 100px without stretching the image*/
        object-fit:cover;
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

    .blog-desc{
      color: #747a7a;
    }
  }
</style>