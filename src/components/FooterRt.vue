<template>
  <footer>
    <div class="foot-contain">
      <div class="address">
        <h3>Address</h3>
        <h4>382 NE 191st St # 87394 Miami FL, 33179-3899</h4>
        <h4>+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)</h4>
        <h5>support@maxcoach.com</h5>
        <span class="social"
          v-for="icon in socialIcon"
          :key="icon.icon"
        >
          <a :href="icon.link"><i class="icons" :class= "icon.icon" /></a>
        </span>
      </div>
      <div class="explore">
        <ul>
          <li class="title">Explore</li>
          <a
            v-for="element in arrExplore"
            :key="element.name"
            :href="element.link"
          >
            <li>{{ element.name }}</li>
          </a>
        </ul>
      </div>
      <div class="about">
        <ul>
          <a
            v-for="element in arrAbout"
            :key="element.name"
            :href="element.link"
          >
            <li>{{ element.name }}</li>
          </a>
        </ul>
      </div>
      <div class="information">
        <ul>
          <li class="title">Information</li>
          <a
            v-for="element in arrInformation"
            :key="element.name"
            :href="element.link"
          >
            <li>{{ element.name }}</li>
          </a>
        </ul>
      </div>
    </div>
    <div class="copyright">
      <span>&copy; 2020 Maxcoach. All Right Reserved</span>
    </div>

    <!-- cerchio verde che rimanda all'inizio della pagina -->
    <div class="circle-up">
      <a href="head-page"><font-awesome-icon icon="fa-solid fa-arrow-up" /></a>
    </div>

  </footer>
</template>

<script>

export default {
  name: 'FooterRt',
  data () {
    return {
      socialIcon: [
        {
          icon: 'fa-brands fa-facebook-square',
          link: '#'
        },
        {
          icon: 'fa-brands fa-twitter',
          link: '#'
        },
        {
          icon: 'fa-brands fa-instagram',
          link: '#'
        },
        {
          icon: 'fa-brands fa-linkedin',
          link: '#'
        }
      ],
      arrExplore: [
        {
          name: 'Start here',
          link: '#'
        },
        {
          name: 'Blog',
          link: '#'
        },
        {
          name: 'About us',
          link: '#'
        }
      ],
      arrAbout: [
        {
          name: 'Success story',
          link: '#'
        },
        {
          name: 'Courses',
          link: '#'
        },
        {
          name: 'Contact us',
          link: '#'
        }
      ],
      arrInformation: [
        {
          name: 'Membership',
          link: '#'
        },
        {
          name: 'Purchase guide',
          link: '#'
        },
        {
          name: 'Privacy policy',
          link: '#'
        },
        {
          name: 'Terms of services',
          link: '#'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";
footer {
  background-color: $hintred-color;
  position: relative;
  li {
    list-style-type: none;
  }
  .foot-contain {
    width: 800px;
    margin: 0 auto;
    display: flex;
    padding: 40px 0;
    .address {
      width: 50%;
      h3 {
        font-size: .9rem;
        margin-bottom: 22px;
      }
      h4,
      h5 {
        font-size: .7rem;
        color: $dovegray-color;
        padding-bottom: 1.5rem;
      }
    }
    .social {
      padding-left: 5px;
      padding-right: 20px;
      a {
        color: $silver-color;
        font-size: 1.3rem;
        text-decoration: none;
      }
      .icons {
        transition: .5s;
      }
    }
    .explore {
      margin-left: 20px;
      margin-right: 10px;
    }
    .about {
      margin-top: 39px;
      margin-left: 30px;
    }
    .information {
      margin-left: 50px;
    }
    .title {
      font-size: .9rem;
      margin-bottom: 20px;
      font-weight: bolder;
    }
    a {
      text-decoration: none;
      color: $dovegray-color;
      font-size: .7rem;
      font-weight: bolder;
      li {
        margin-bottom: 25px;
      }
    }
  }
  .copyright {
    text-align: center;
    color: $silver-color;
    font-size: .8rem;
    padding-bottom: 40px;
  }
  .circle-up {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background-color: $jungle-green;
    display: flex;
    justify-content: center;
    margin: 20px;
    position: absolute;
    bottom: 0;
    right: 0;
    overflow: hidden;
    background-size: 400% 400%;
    animation: TransitioningBackground 5s ease infinite;
    transition: 4s;
    &::before {
      content: '';
      display: block;
      position: absolute;
      background: rgba(255, 255, 255, 0.5);
      width: 60px;
      height: 100%;
      top: 0;
      filter: blur(30px);
      transform: translateX(-100px) skewX(-15deg);
    }
    &::after {
      content: '';
      display: block;
      position: absolute;
      background: rgba(255, 255, 255, 0.2);
      height: 100%;
      top: 0;
      filter: blur(5px);
      transform: translateX(-100px) skewX(-15deg);
    }
    &:hover {
      background-image: (linear-gradient(to left, #2d8fe5, #d155b8));
      cursor: pointer;
      &::before,
      &::after {
        transform: translateX(100px) skewX(-15deg);
        transition: 5s;
      }
    }
  }
    a {
      align-self: center;
      color: $white-color;
    }
  }
  .social:hover .icons{
    transform: scale(1.2);
    transition: .5s;
  }
  @keyframes TransitioningBackground {
  0% {
    background-position: 1% 0%;
  }
  50% {
    background-position: 99% 100%;
  }
  100% {
    background-position: 1% 0%;
  }
}
</style>
