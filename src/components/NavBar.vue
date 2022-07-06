<template>
  <section class="navbar">
    <nav class="navbar-wrapper">
      <div class="nav-logo">
        <a href="#">Aurora</a>
      </div>
      <div class="nav-links">
        <ul>
          <li>Demos</li>
          <li>Style Guide</li>
          <li>Membership</li>
          <li>Join</li>
        </ul>
      </div>
    </nav>
  </section>
</template>

<script>
  export default{
    name: "NavBar",
    props: {
      items: Array,
    },
  }
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Alegreya+Sans+SC:wght@100;400&display=swap');
  .navbar{
    padding: 10px 0;
    .navbar-wrapper {
      display: flex;
      justify-content: space-between;
      align-items: center;

      .nav-logo {
        a {
          text-decoration: none;
          font-family: 'Alegreya Sans SC', sans-serif;
          color: black;
          font-size: 50px;
        }

      }

      .nav-links{
        ul{
          //text-decoration: none;
          list-style: none;

          li{
              display: inline-block;
              margin: 0 10px;
              font-family: 'Inter', sans-serif;
          }
        }
      }
    }

  }
</style>