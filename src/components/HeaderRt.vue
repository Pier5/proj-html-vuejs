<template>
  <header id="head-page">
    <div class="head-container">
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
  .head-container {
    width: 950px;
    display: flex;
    align-items: center;
    margin: 0 auto;
}
  .fa-cart-shopping,
  .fa-circle-user {
    color: $white-color;
    align-self: flex-end;
    font-size: .9rem;
    font-weight: bolder;
    margin-left: 5px;
    cursor: pointer;
  }
  .fa-circle-user {
    align-self: center;
    font-size: 1rem;
  }
  .head-logo {
    width: 15%;
    margin-right: auto;
    cursor: pointer;
  }
  .nav-head {
    display: flex;
    align-items: center;
    height: 100%;
    .list-item {
      display: inline-block;
      margin-left: 35px;
      cursor: pointer;
     .link-item {
        color: $white-color;
        text-decoration: none;
        font-size: .75rem;
        font-weight: bolder;
      }
      .fa-angle-down {
        color: $white-color;
        font-size: .5rem;
        margin-left: 4px;
      }
    }
    .cart {
      position: relative;
      margin-right: 30px;
      .cart-items {
        width: 12px;
        height: 12px;
        color: $white-color;
        background-color: $white-color;
        display: flex;
        justify-content: center;
        align-items: center;
        color: black;
        border-radius: 50%;
        font-size: .5rem;
        position: absolute;
        top: -6px;
        right: -7px;
      }
    }
    .input-search {
      background-color: white;
      margin-left: 20px;
      border-radius: .4rem;
      padding: .3rem;
      .search-bar {
        font-size: .7rem;
        border: none;
        padding: .4rem;
      }
      .fa-magnifying-glass {
        font-size: .8rem;
        color: $mountain-meadow;
        padding-left: .2rem;
      }
    }
  }
  .list-item:hover .link-item {
    color: $mountain-meadow;
  }
  .list-item:hover .fa-angle-down {
    color: $mountain-meadow;
  }
  .cart:hover .cart-items {
    background-color: gold;
  }
  .cart:hover .fa-cart-shopping {
    color: $mountain-meadow;
  }
  .fa-circle-user:hover {
    color: $mountain-meadow;
  }
}
</style>
