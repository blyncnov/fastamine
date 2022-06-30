<template>
  <div class="Navigation__Container">
    <div class="Fastanime__max__width">
      <div class="Navigation__Section">
        <!-- Logo Section -->
        <div class="Navigation__Logo">
          <h1>
            {{ Logo }}<span>{{ LogoSubString }}</span>
          </h1>
        </div>

        <!-- Navigation List Items -->
        <ul>
          <li v-for="list in NavigationList" :key="list.id">
            <a href="/">{{ list.name }}</a>
          </li>
        </ul>

        <div class="Right__Profile">
          <!-- Search For Movies -->
          <div class="Search__Container">
            <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
            <input
              class="search__input"
              type="text"
              placeholder="Search for movies...."
            />
          </div>

          <!-- Profile Card -->
          <div class="ProfileHandle__Container">
            <div class="Profile__circle"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navigation",

  data() {
    return {
      Logo: "Fast",
      LogoSubString: "anime",
      NavigationList: [
        {
          name: "Home",
          url: "/",
        },
        {
          name: "Movies",
          url: "/movies",
        },
        {
          name: "News",
          url: "/news",
        },
        {
          name: "Blog",
          url: "/blog",
        },
        {
          name: "My List",
          url: "/list",
        },
        {
          name: "About",
          url: "/about",
        },
        {
          name: "Contact",
          url: "/contact",
        },
      ],
    };
  },
};
</script>

<style lang="scss"  scoped>
.Navigation__Container {
  width: 100%;
  flex: 1;
  background-color: transparent;
}

.Navigation__Section {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1em 0;

  .Navigation__Logo {
    h1 {
      color: white;
      font-size: 20px;

      span {
        color: salmon;
      }
    }
  }
}

ul {
  display: flex;
  gap: 1.5em;

  li {
    color: rgb(238, 237, 237);
    font-size: 13px;
  }

  @media (max-width: 768px) {
    display: none;
  }
}

.Right__Profile {
  display: flex;
  justify-content: flex-end;
  align-items: center;

}

.Profile__circle {
  width: 30px;
  height: 30px;
  border-radius: 49.5%;
  background-color: white;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;

   @media (max-width: 768px) {
    display: none;
  }
}

.Search__Container {
  display: flex;
  align-items: center;
  gap: 0.5em;
  color: white;

  .search__input {
    border: none;
    background-color: transparent;
    color: white;
    font-size: 13px;
    width: 100%;
  }
}
</style>