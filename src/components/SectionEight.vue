<template>
  <section class="section-eight">
    <div class="circle circle-one"></div>
    <div class="circle circle-two"></div>
    <div class="circle circle-reverse circle-three"></div>
    <div class="courses">
      <div class="details"
        v-for="element in arrCourses"
        :key="element.title"
      >
        <font-awesome-icon :icon= "element.icon" class="icon" />
        <h2>{{ element.title }}</h2>
        <h3>{{ element.text }}</h3>
      </div>
    </div>
    <img class="img-jumbo" src="../assets/img/home-6-services-image-768x308.png" alt="">
  </section>
</template>

<script>
export default {
  name: 'section-eight',
  data () {
    return {
      arrCourses: [
        {
          icon: 'fa-regular fa-flag',
          title: 'Idea Discussion',
          text: 'Get teamed up with the specialists who work and teach coding for years at famous universities.'
        },
        {
          icon: 'fa-solid fa-gear',
          title: 'Web Development',
          text: 'Learn to start building a webpage from scratch. You decide your own pace, course and speed.'
        },
        {
          icon: 'fa-regular fa-life-ring',
          title: 'System Administration',
          text: 'Learners are encouraged to study the mechanism and structure of system administration.'
        },
        {
          icon: 'fa-solid fa-display',
          title: 'Graphic Design',
          text: 'Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";

.section-eight {
  height: 600px;
  margin-bottom: 40px;
  font-family: 'Quicksand', sans-serif;
  position: relative;
  box-shadow: rgba(211, 208, 208, 0.38) 0 -560px 236px -120px inset;
  .circle {
    position: absolute;
    border-radius: 50%;
  }
  .circle-one {
    width: 30px;
    height: 30px;
    background-color: #fa7d61;
    bottom: 40px;
    left: 60px;
  }
  .circle-two {
    width: 35px;
    height: 35px;
    background-color: #bce6df;
    bottom: 260px;
    left: 1150px;
  }
  .circle-three {
    width: 40px;
    height: 40px;
    background-color: transparent;
    border: 5px solid #bce6df;
    bottom: 350px;
    left: 400px;
  }
  .circle {
    animation: circleMove 4s linear infinite;
  }
  .circle-reverse {
    animation: circleMoveReverse 4s linear infinite;
  }
  @keyframes circleMove {
    from {
      transform: rotate(0deg) translateX(50px) rotate(0deg);
    }
    to   {
      transform: rotate(360deg) translateX(50px) rotate(-360deg);
    }
  }
  @keyframes circleMoveReverse {
    from {
      transform: rotate(0deg) translateX(50px) rotate(0deg);
    }
    to   {
      transform: rotate(-360deg) translateX(50px) rotate(360deg);
    }
  }
  .courses {
    width: 900px;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    padding-left: 85px;
    .details {
      margin-top: 30px;
      width: calc(100% / 4);
      padding-right: 30px;
      .icon {
        font-size: 2rem;
      }
      h2 {
        font-size: .9rem;
        margin: 15px 0 10px;
      }
      h3 {
        font-size: .6rem;
        line-height: 1.1rem;
        color: $dovegray-color;
      }
    }
  }
  .img-jumbo {
    width: 50%;
    position: absolute;
    bottom: 0;
    left: 0;
    transform: translate(52%, 7%);
  }
}
</style>
