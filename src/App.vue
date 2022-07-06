<template>
<!--  <img alt="Vue logo" src="./assets/logo.png">-->
<!--  <HelloWorld msg="Welcome to Your Vue.js App"/>-->
  <div class="container">
    <NavBar/>
    <HeaderSection/>
    <RecentBlogs :items="items"/>
  </div>

</template>

<script>
import NavBar from "@/components/NavBar";
import HeaderSection from "@/components/HeaderSection";
// import BlogItem  from "@/components/BlogItem";
import RecentBlogs from "@/components/RecentBlogs";

export default {
  name: 'App',
  components: {
    // BlogItem,
    HeaderSection,
    NavBar,
    RecentBlogs,
  },
  data(){
    return {
      items: [
        {
          title: "Title 1",
          desc: "Desc 1",
          img: "https://unsplash.com/photos/weOhm0rb1ds/download?ixid=MnwxMjA3fDB8MXxhbGx8N3x8fHx8fDJ8fDE2NTcxMzk0Mzc&force=true&w=640",
          tags: [
            "Lifestyle","People","Review"
          ]
        }

      ]
    }
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;400;700&display=swap');
*{
  margin:0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.container{
  width: 95%;
  margin:0 auto;
}


</style>
