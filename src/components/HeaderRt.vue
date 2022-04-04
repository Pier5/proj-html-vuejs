<template>
  <header id="head-page">
    <div class="container">
      <img class="head-logo" src="../assets/img/light-logo.png" alt="logo azienda MaxCoach">
      <nav class="nav-head">
        <ul>
          <li class="list-item" v-for="item in arrNavBar" :key="item">
            <a class="link-item" href="item.link">{{ item.text }}</a>
            <font-awesome-icon icon="fa-solid fa-angle-down" />
          </li>
        </ul>
        <div class="cart">
          <font-awesome-icon icon="fa-solid fa-cart-shopping" />
          <div class="cart-items"><span class="items-add">0</span></div>
        </div>
        <font-awesome-icon icon="fa-regular fa-circle-user" />
        <div class="input-search">
          <input class="search-bar" type="text" placeholder="Search..">
          <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
        </div>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderRt',
  data () {
    return {
      arrNavBar: [
        {
          text: 'Home',
          link: '#'
        },
        {
          text: 'Pages',
          link: '#'
        },
        {
          text: 'Courses',
          link: '#'
        },
        {
          text: 'Features',
          link: '#'
        },
        {
          text: 'Blog',
          link: '#'
        },
        {
          text: 'Shop',
          link: '#'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";

header {
  width: 100%;
  height: 5rem;
  background-color: $portgore-color;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  position: fixed;
  z-index: 5;
  .fa-cart-shopping,
  .fa-circle-user {
    color: $white-color;
    align-self: flex-end;
    font-size: 1.1rem;
    margin-left: 8px;
    cursor: pointer;
  }
  .fa-circle-user {
    align-self: center
  }
  .head-logo {
    width: 12%;
    margin-right: auto;
  }
  .nav-head {
    display: flex;
    align-items: center;
    height: 100%;
    .list-item {
      display: inline-block;
      margin-left: 40px;
      cursor: pointer;
     .link-item {
        color: $white-color;
        text-decoration: none;
        font-size: .9rem;
        font-weight: bolder;
      }
      .fa-angle-down {
        color: $white-color;
        font-size: .6rem;
        margin-left: 5px;
      }
    }
    .cart {
      position: relative;
      margin-right: 30px;
      .cart-items {
        width: 15px;
        height: 15px;
        color: $white-color;
        background-color: $white-color;
        display: flex;
        justify-content: center;
        align-items: center;
        color: black;
        border-radius: 50%;
        font-size: .6rem;
        position: absolute;
        top: -10px;
        right: -10px;
      }
    }
    .input-search {
      background-color: white;
      margin-left: 20px;
      border-radius: .4rem;
      padding: .4rem;
      .search-bar {
        border: none;
        padding: .4rem 0;
      }
      .fa-magnifying-glass {
        color: $mountain-meadow;
        padding-left: .2rem;
      }
    }
  }
}
</style>
