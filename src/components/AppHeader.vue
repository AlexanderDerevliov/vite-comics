
<script>
export default {
  data() {
    return {
      itemMenu: [
        "Characters",
        "Comics",
        "Movies",
        "Tv",
        "Games",
        "Videos",
        "Fans",
        "Shop",
      ],
    }
  }
}


</script>


<template>
  <header class="header">
    <div class="header-top"></div>
    <div class="container">
      <nav class="header-bottom">
        <div class="logo">
          <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <ul>
          <li v-for="item in itemMenu" :key="item"><a href="">{{ item }}</a></li>
        </ul>
      </nav>
    </div>

  </header>
</template>

<style  lang="scss" scoped>
@use "../style/partials/variables.scss" as*;

.header {

  &-top {
    background-color: rgb(35, 34, 34);
    height: 30px;
  }

  &-bottom {
    display: flex;
    justify-content: space-between;
    direction: row;
    align-items: center;
    flex-wrap: nowrap;
    padding: 1rem;
  }

  ul {
    display: flex;
    align-items: center;
    gap: 1rem;

    li {
      list-style-type: none;
    }

    a {
      color: black;
      text-decoration: none;
    
      &:hover {
        background-color: lightblue;
        padding: .5rem;
        border-radius: 10px;
      }
    }
  }

}

.container {
  width: 95%;
  margin: 0 auto;
}
</style>