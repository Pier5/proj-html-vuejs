<template>
  <section class="section-six">
    <div class="blog">
      <div class="blog-text">Enjoy reading on Maxcoach</div>
      <h1>Latest On <span class="green-text">Our Blogs</span></h1>
      <div class="container-blog">
        <div class="blog-post"
          v-for="post in blogPosts"
          :key="post"
        >
          <a :href="post.link"><img class="blog-img" :src="post.img" :alt="post.title"></a>
          <h3>{{ post.profession }}</h3>
          <a :href="post.link"><h2>{{ post.title }}</h2></a>
          <span class="date"><font-awesome-icon icon="fa-regular fa-calendar" />{{ post.date }}</span>
          <span class="viewers"><font-awesome-icon icon="fa-solid fa-eye" />{{ post.views }}</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import imgOne from '../assets/img/artist-blog-03-480x325.jpeg'
import imgTwo from '../assets/img/artist-blog-01-480x325.jpg'
import imgThree from '../assets/img/artist-blog-02-480x325.jpg'

export default {
  name: 'SectionSix',
  data () {
    return {
      blogPosts: [
        {
          img: imgOne,
          link: '#',
          profession: 'Artist',
          title: 'Brush Strokes Energize Trees in Paintings',
          date: 'May 15, 2020',
          views: '688'
        },
        {
          img: imgTwo,
          link: '#',
          profession: 'Artist',
          title: 'Pocket-Sized Notebooks Hold Miniature Paintings',
          date: 'May 15, 2020',
          views: '603'
        },
        {
          img: imgThree,
          link: '#',
          profession: 'Artist',
          title: 'Connection Between Self-Portraits and Identity',
          date: 'May 15, 2020',
          views: '397'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";
.section-six {
  background-color: $hintred-color;
  .blog {
    width: 700px;
    text-align: center;
    margin: 0 auto;
    .blog-text {
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
    .container-blog {
      display: flex;
      width: 800px;
      .blog-post {
        margin: 20px 15px 60px 0;
        width: calc(100% / 3 - 30px);
        text-align: left;
        .blog-img {
          width: 100%;
          border-radius: 3px;
        }
        h3 {
          margin: 15px 0 10px;
          font-size: .6rem;
          text-transform: uppercase;
          color: $dovegray-color;
          letter-spacing: 2px;
        }
        a {
          text-decoration: none;
          color: black;
        }
        h2 {
          font-size: 1rem;
          margin-bottom: 12px;
        }
        .date,
        .viewers {
          font-size: .6rem;
          font-family: 'Quicksand', sans-serif;
          color: $dovegray-color;
          margin-right: 20px;
          .fa-eye,
          .fa-calendar {
            margin-right: 5px;
          }
        }
      }
    }
  }
}
</style>
