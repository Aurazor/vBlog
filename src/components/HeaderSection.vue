<template>
  <header>
    <p><span>Hey, we're Aurora.</span> See our thoughts, stories and ideas.</p>
  </header>
</template>

<script>
export default {
  name: "HeaderSection"
}
</script>

<style lang="scss" scoped>
  header{
    font-family: 'Inter', sans-serif;
    font-size: 61px;
    display: flex;
    justify-content: center;
    align-items: center;

    p{
      span{
        font-weight: bold;
        background: linear-gradient(to bottom left, #94F568, #2959A7);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
      }
    }
  }
</style>