<template>
  <div class="Hero__Container">
    <div class="Hero__Section">
      <div class="Hero__Left__Side">
        <div class="Hero__Column">
          <div class="Hero__Flex">
            <div class="Hero__max__width">
              <div class="Hero__Text">
                <h1>Spider man : <span>Far From Home </span></h1>
                <div class="Hero__Tagline">
                  <h4>
                    Coming Soon : <span>Wednesdays, June 3rd, 18:40</span>
                  </h4>
                </div>
                <div class="Hero__Button__Container">
                  <button class="button btn-1">Watch Trailer</button>
                  <button class="button btn-2">Add List</button>
                </div>
              </div>
            </div>
            <br />
            <div class="Hero__About__Category">
              <div class="Hero__max__width">
                <Category />
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="Hero__Right__Side">
        <div class="Hero__max__width">
          <div class="Hero__Column">
            <div>
              <div class="Hero__Post">
                <h1>Men IN BLACK</h1>
                <p>
                  Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                  Nobis excepturi error nulla! Hic quo aliquam saepe, similique
                  accusamus.
                </p>
              </div>
              <div class="Hero__Post">
                <h1><span></span> SPIDER MAN : FAR FROM HOME</h1>
                <p>
                  Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                  Nobis excepturi error nulla! Hic quo aliquam saepe, similique
                  accusamus.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Category from "./Category.vue";
export default {
  components: { Category },
};
</script>

<style lang="scss" scoped>
.Hero__Container {
  padding: 30px 0 0 0;
  flex: 3;
}

.Hero__Flex {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.Hero__Section {
  width: 100%;
  display: grid;
  grid-template-columns: 1fr 1fr;
  line-height: 1.5;
  gap: 1em;

  @media (max-width: 768px) {
    grid-template-columns: 1fr;
  }
}

.Hero__Text {
  h1 {
    font-size: 3rem;
    font-weight: bold;
    color: #fff;
    line-height: 1.1 !important;
  }

  h4 {
    margin: 1em 0;
    font-size: 1rem;
    font-weight: 300;
    color: rgb(218, 218, 218);
  }
}

.Hero__max__width {
  max-width: 100%;
  padding-left: 10%;

  @media (max-width: 768px) {
    padding-left: 5%;
  }
}

.Hero__Button__Container {
  display: flex;
  align-items: center;
  margin: 1em 0;
  gap: 1.5em;
}

.button {
  background-color: #fff;
  border: none;
  padding: 0.5em 1em;
  border-radius: 4px;
  font-size: 1rem;
  font-weight: bold;
  color: #333333;
  cursor: pointer;
}

.btn-1 {
  background-color: salmon;
  color: #fff;
}

.Hero__About__Category {
  width: 100%;
  padding: 1.5em 0 1.5em;
  background-color: #9187ff3e;
  border-radius: 0 4em 0 0;
  color: white;
  margin-top: 2em;

  @media (max-width: 768px) {
     border-radius: 0 3em 3em 0;
  }
}

.Hero__Column {
  color: white;
  padding-right: 10%;

  @media (max-width: 768px) {
    padding-right: 5%;
  }
}

.Hero__Post {
  margin-bottom: 1em;
 

  h1 {
    span {
      width: 30px;
      height: 30px;
      background-color: salmon;
    }
  }

  p {
    font-size: 12px;
    font-weight: 300;
    color: rgb(218, 218, 218);
  }
}
</style>