<template>
  <header>
    <div class="container">
      <img class="head-logo" src="../assets/img/light-logo.png" alt="logo azienda MaxCoach">
      <nav>
        <ul>
          <li class="list-item" v-for="item in arrNavBar" :key="item">
            <a class="link-item" href="item.link">{{ item.text }}</a>
            <i class="fa-solid fa-angle-down"></i>
          </li>
        </ul>
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
@import "../assets/styles/partials/variables.scss";

header {
  width: 100%;
  height: 5rem;
  background-color: $rhino-color;
  display: flex;
  align-items: center;
  .head-logo {
    width: 10%;
    margin-right: auto;
  }
  .list-item {
    display: inline-block;
    margin-right: 40px;
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

}
</style>
