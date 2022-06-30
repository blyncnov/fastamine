<template>
  <div class="category__Section">
    <div class="category__Details">
      <h1>CATEGORY</h1>
      <p>
        lorem ipsum dolor sit amet lorem ipsum dolor lorem ipsum dolor sit amet
        lorem ipsum dolor
      </p>
    </div>
    <div class="category__Details">
      <h1>STORYLINE</h1>
      <p>lorem ipsum dolor sit amet lorem ipsum dolor</p>
    </div>
    <div class="category__Details">
      <h1>DIRECTOR / WRITER</h1>
      <p>
        lorem ipsum dolor sit amet lorem ipsum dolor lorem ipsum dolor sit amet
        lorem ipsum dolor
      </p>
    </div>
    <div class="category__Details">
      <h1>STARS</h1>
      <p>
        lorem ipsum dolor sit amet lorem ipsum dolor lorem ipsum dolor sit amet
        lorem ipsum dolor
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.category__Section {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 2em;
  padding: 0 1em 0 0;
  align-self: center;
}

.category__Details {
  h1 {
    font-weight: bold;
    color: #fff;
  }

  p {
    font-size: 12px;
    font-weight: 300;
    opacity: 0.8;
    color: rgb(218, 218, 218);
  }
}
</style>