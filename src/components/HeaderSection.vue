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
    font-size: 78px;
    display: flex;
    justify-content: center;
    align-items: center;

    p{
      span{
        font-weight: bold;
      }
    }
  }
</style>