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
          title: "Creating is a privilege but it’s also a gift",
          desc: "Nullam vel lectus vel velit pellentesque dignissim nec id magna. Cras molestie ornare quam at semper. Proin a ipsum ex. Curabitur eu",
          img: "https://unsplash.com/photos/weOhm0rb1ds/download?ixid=MnwxMjA3fDB8MXxhbGx8N3x8fHx8fDJ8fDE2NTcxMzk0Mzc&force=true&w=640",
          tags: [
            "Lifestyle","People","Review"
          ]
        },
        {
          title: "Being unique is better than being perfect",
          desc: "Nam in pretium dui. Phasellus dapibus, mi at molestie cursus, neque eros aliquet nisi, non efficitur nisi est nec mi. Nullam semper, ligula a",
          img: "https://unsplash.com/photos/R98l5I6OFQY/download?ixid=MnwxMjA3fDF8MXxhbGx8NDZ8fHx8fHwyfHwxNjU3MjI5NDE4&force=true&w=640",
          tags: [
            "Lifestyle","People","Review"
          ]
        },
        {
          title: "Now we’re getting somewhere",
          desc: "Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Donec volutpat rhoncus quam, a feugiat elit",
          img: "https://unsplash.com/photos/UBEkSqIpwlY/download?ixid=MnwxMjA3fDB8MXxhbGx8NTh8fHx8fHwyfHwxNjU3MjI5NDIx&force=true&w=640",
          tags: [
            "Lifestyle","People","Review"
          ]
        },
        {
          title: "The trick to getting more done is to have the freedom to roam around",
          desc: "Integer nec mi cursus, blandit est et, auctor mauris. Aenean ex metus, faucibus in mattis at, tincidunt eu dolor. Cras hendrerit massa nec",
          img: "https://unsplash.com/photos/4CaVbHUXf5o/download?ixid=MnwxMjA3fDF8MXxhbGx8ODZ8fHx8fHwyfHwxNjU3MjMxMjIy&force=true&w=640",
          tags: [
            "Lifestyle","People","Review"
          ]
        },
        {
          title: "Your voice, your mind, your story, your vision",
          desc: "Nullam auctor nisi non tortor porta, id dapibus lectus rhoncus. Vivamus lobortis posuere enim finibus sodales. Phasellus quis tellus",
          img: "https://unsplash.com/photos/tel_aGfrN4w/download?ixid=MnwxMjA3fDB8MXxhbGx8MTE5fHx8fHx8Mnx8MTY1NzIzMTI1Mw&force=true&w=640",
          tags: [
            "Lifestyle","People","Review"
          ]
        },
        {
          title: "Every day, in every city and town across the country",
          desc: "Morbi a facilisis lectus. Ut eu dapibus risus, a interdum justo. Vestibulum volutpat velit ac tellus mollis, sit amet sodales metus elementum.",
          img: "https://unsplash.com/photos/VdN2CGmvM88/download?ixid=MnwxMjA3fDB8MXxhbGx8MTI0fHx8fHx8Mnx8MTY1NzIzMTI1OQ&force=true&w=640",
          tags: [
            "Lifestyle","People","Review"
          ]
        },

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
