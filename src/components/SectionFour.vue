<template>
  <section class="section-four">
    <div class="course-card">
      <div class="course-text">Choose a course to get started</div>
      <h1>Latest Featured <span class="green-text">Courses</span></h1>
      <div class="cards">
        <div class="card"
          v-for="info in infoCourses"
          :key="info.description"
        >
          <img class="circle" :src="info.img" :alt="info.description">
          <div class="infos">
            <h3 class="price">{{ info.price }}</h3>
            <h4 class="card-text">{{ info.description }}</h4>
            <span class="lesson"><font-awesome-icon icon="fa-regular fa-file-lines" />{{ info.lesson }}</span>
            <span class="students"><font-awesome-icon icon="fa-regular fa-user" />{{ info.students }}</span>
          </div>
        </div>
      </div>
      <button class="main-btn">View all courses<font-awesome-icon icon="fa-solid fa-arrow-right-long" /></button>
    </div>
  </section>
</template>

<script>
import img1 from '../assets/img/course-02-480x298.jpg'
import img2 from '../assets/img/stock-full-hd-03-480x298.jpg'
import img3 from '../assets/img/stock-full-hd-04-480x298.jpg'
import img4 from '../assets/img/stock-full-hd-06-480x298.jpg'
import img5 from '../assets/img/course-featured-image-01-480x298.jpg'
import img6 from '../assets/img/stock-full-hd-05-480x298.jpg'

export default {
  name: 'SectionFour',
  data () {
    return {
      infoCourses: [
        {
          img: img1,
          price: '$40.oo',
          description: 'Learning to Write as a Professional Author',
          lesson: '20 lessons',
          students: '50 students'
        },
        {
          img: img2,
          price: 'Free',
          description: 'Customer-centric Info-Tech Strategies',
          lesson: '24 lessons',
          students: '769 students'
        },
        {
          img: img3,
          price: '$19.oo',
          description: 'Open Programming Courses for Everyone: Python',
          lesson: '17 lessons',
          students: '62 students'
        },
        {
          img: img4,
          price: '$26.oo',
          description: 'Accademic Listening and Note-taking',
          lesson: '14 lessons',
          students: '67 students'
        },
        {
          img: img5,
          price: '$39.oo',
          description: 'Master jQuery in a Short Period of Time',
          lesson: '6 lessons',
          students: '51 students'
        },
        {
          img: img6,
          price: '$59.oo',
          description: 'Introduction to Javascript for Beginners',
          lesson: '14 lessons',
          students: '76 students'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";

.section-four {
  background-color: $lightheavenly;
  .course-card {
    width: 700px;
    text-align: center;
    margin: 0 auto;
    .course-text {
      font-size: .7rem;
      color: $dovegray-color;
      text-transform: uppercase;
      padding-top: 50px
    }
    h1 {
      margin: 1rem 0 1.6rem;
      font-size: 1.8rem;
      line-height: 2rem;
      .green-text {
        color: $mountain-meadow;
        font-weight: lighter;
      }
    }
    .cards {
      display: flex;
      flex-wrap: wrap;
      margin-top: 30px;
      .card {
        width: 340px;
        display: flex;
        margin: 20px 5px;
        padding: 10px;
        cursor: pointer;
        .circle {
          width: 100px;
          height: 100px;
          border-radius: 50%;
          object-fit: cover;
          margin-right: 15px;
        }
      }
      .infos {
        text-align: left;
        .price {
          font-size: .9rem;
          color: $jungle-green;
        }
        .card-text {
          font-size: .8rem;
          margin: 10px 0;
        }
        .lesson {
          font-size: .6rem;
          margin-right: 15px;
          color: $shady-color;
          .fa-file-lines {
            margin-right: 5px;
          }
        }
        .students {
          font-size: .6rem;
          color: $shady-color;
          .fa-user {
            margin-right: 5px;
          }
        }
      }
    }
    .main-btn {
      border: none;
      background-color: $mountain-meadow;
      color: $white-color;
      font-weight: bolder;
      font-size: .7rem;
      padding: .6rem 1.2rem;
      border-radius: 3px;
      margin-top: 20px;
      margin-bottom: 55px;
      font-family: 'Quicksand', sans-serif;
      cursor: pointer;
      .fa-arrow-right-long {
        margin-left: 5px;
        font-size: .7rem;
      }
    }
  }
  .card:hover {
          background-color: white;
        }
}
</style>
