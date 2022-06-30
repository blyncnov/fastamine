<template>
  <div>
    <h1>My Section {{ myData }} {{Props}} </h1>
  </div>
</template>

<script>
export default {
  props: ["myData", "Props"],
};
</script>

<style lang="scss" scoped>
</style>