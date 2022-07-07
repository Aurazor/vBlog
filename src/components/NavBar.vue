<template>
  <section class="navbar">
    <nav class="navbar-wrapper">
      <div class="nav-logo">
        <a href="#">Aurora</a>
      </div>
      <div class="nav-links">
        <ul>
          <li>Home</li>
          <li>New</li>
          <li>Login</li>
          <li>Sign Up</li>
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
              cursor: pointer;
              transition: 0.5s ease;

            &:hover{
              text-decoration: underline;
              background: linear-gradient(to bottom left, #94F568, #2959A7);
              -webkit-background-clip: text;
              -webkit-text-fill-color: transparent;
            }
          }
        }
      }
    }

  }
</style>