<template>
  <div class="Header__Container">
    <Navigation />
    <Hero />
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      message: "Hello Vue!",
    };
  },
};
</script>

<style lang="scss" scoped>
.Header__Container {
  position: relative;
  background-color: #131637;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100vh;

  @media (max-width: 768px) {
    height: auto !important;
  }
}
</style>