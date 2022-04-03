<template>
  <section class="section-five">
    <div class="partners">
      <h1>Why People Talk About <span class="green-text">MaxCoach</span>?</h1>
      <div class="quote">
        <div class="circles">
          <img src="../assets/img/testimonial-avata-02.jpg" alt="mina hollace" class="circle">
          <img src="../assets/img/maxcoach-shape-05-100x100.png" alt="cerchio" class="under-circle">
        </div>
        <div class="quote-text">
          <h2>I am free to learn at my own pace, follow my own schedule and choose the subject I like. Great study portal for people like me.</h2>
          <h3>Mina Hollace</h3>
          <h4>/ Freelancer</h4>
        </div>
      </div>
      <div class="clients">
        <div class="client"
          v-for="element in logoClients"
          :key="element"
        >
        <a :href="element.link"><img :src="element.logo" :alt="element.text" class="logos"></a>
      </div>
      </div>
    </div>
  </section>
</template>

<script>
import logo1 from '../assets/img/client-logo-colored-01.png'
import logo2 from '../assets/img/client-logo-colored-02.png'
import logo3 from '../assets/img/client-logo-colored-03.png'
import logo4 from '../assets/img/client-logo-colored-04.png'
import logo5 from '../assets/img/client-logo-colored-05.png'
import logo6 from '../assets/img/client-logo-colored-06.png'

export default {
  name: 'SectionFive',
  data () {
    return {
      logoClients: [
        {
          logo: logo1,
          link: '#',
          text: 'acqua'
        },
        {
          logo: logo2,
          link: '#',
          text: 'adRoll'
        },
        {
          logo: logo3,
          link: '#',
          text: 'firefox'
        },
        {
          logo: logo4,
          link: '#',
          text: 'woodland'
        },
        {
          logo: logo5,
          link: '#',
          text: 'bullfit'
        },
        {
          logo: logo6,
          link: '#',
          text: 'sixbase'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";
.partners {
  width: 700px;
  margin: 50px auto;
  text-align: center;
  h1 {
    margin: 1rem 0 1.6rem;
    font-size: 1.8rem;
    line-height: 2rem;
    .green-text {
      color: $mountain-meadow;
      font-weight: lighter;
    }
  }
  .quote {
    margin-top: 50px;
    display: flex;
    .circles {
      width: 30%;
      margin-left: 20px;
      margin-right: 20px;
      position: relative;
      .circle {
        position: relative;
        width: 125px;
        height: 125px;
        border-radius: 50%;
        object-fit: cover;
        z-index: 1;
      }
      .under-circle {
        position: absolute;
        top: 80px;
        right: 40px;
        width: 40%;
        z-index: 0;
      }
    }
    .quote-text {
      width: 70%;
      text-align: left;
      h2 {
        font-size: 1.5rem;
        font-weight: lighter;
      }
      h3 {
        text-transform: uppercase;
        margin-top: 20px;
        font-size: .7rem;
      }
      h4 {
        margin-top: 10px;
        color: $silver-color;
        font-size: .6rem;
      }
    }
  }
  .clients {
    display: flex;
    margin: 70px 0;
    .client {
      margin-left: 45px;
      align-self: center;
    }
    .logos {
      width: 80%;
      margin-right: 80px;
    }
  }
}
</style>
