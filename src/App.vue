<template>
  <div id="app">

    <!-- header -->
    <Header/>

    <!-- main -->
    <main class="main">
      <div class="container">


        <!-- title -->
        <div class="module">
          <h1>Vue.js Application</h1>
        </div>


        <!-- carousel -->
        <div class="module">
          <Flickity :options="{
              prevNextButtons: false,
              pageDots: true,
              selectedAttraction: .15,
              friction: .85,
              lazyLoad: 1
            }" class="carousel">

            <div class="carousel__item">
              <div class="carousel__item-inner image-box">
                <img 
                  data-flickity-lazyload-srcset="https://picsum.photos/640/480/?image=671 640w, https://picsum.photos/480/360/?image=671 480w"
                  sizes="(min-width: 480px) 640px, 480px"
                  data-flickity-lazyload-src="https://picsum.photos/640/480/?image=671"
                  alt=""
                >
              </div>
            </div>

            <div class="carousel__item">
              <div class="carousel__item-inner image-box">
                <img 
                  data-flickity-lazyload-srcset="https://picsum.photos/640/480/?image=289 640w, https://picsum.photos/480/360/?image=289 480w"
                  sizes="(min-width: 480px) 640px, 480px"
                  data-flickity-lazyload-src="https://picsum.photos/640/480/?image=289"
                  alt=""
                >
              </div>
            </div>

            <div class="carousel__item">
              <div class="carousel__item-inner image-box">
                <img 
                  data-flickity-lazyload-srcset="https://picsum.photos/640/480/?image=83 640w, https://picsum.photos/480/360/?image=83 480w"
                  sizes="(min-width: 480px) 640px, 480px"
                  data-flickity-lazyload-src="https://picsum.photos/640/480/?image=83"
                  alt=""
                >
              </div>
            </div>

            <div class="carousel__item">
              <div class="carousel__item-inner image-box">
                <img 
                  data-flickity-lazyload-srcset="https://picsum.photos/640/480/?image=71 640w, https://picsum.photos/480/360/?image=71 480w"
                  sizes="(min-width: 480px) 640px, 480px"
                  data-flickity-lazyload-src="https://picsum.photos/640/480/?image=71"
                  alt=""
                >
              </div>
            </div>

            <div class="carousel__item">
              <div class="carousel__item-inner image-box">
                <img 
                  data-flickity-lazyload-srcset="https://picsum.photos/640/480/?image=816 640w, https://picsum.photos/480/360/?image=816 480w"
                  sizes="(min-width: 480px) 640px, 480px"
                  data-flickity-lazyload-src="https://picsum.photos/640/480/?image=816"
                  alt=""
                >
              </div>
            </div>

            <div class="carousel__item">
              <div class="carousel__item-inner image-box">
                <img 
                  data-flickity-lazyload-srcset="https://picsum.photos/640/480/?image=344 640w, https://picsum.photos/480/360/?image=344 480w"
                  sizes="(min-width: 480px) 640px, 480px"
                  data-flickity-lazyload-src="https://picsum.photos/640/480/?image=344"
                  alt=""
                >
              </div>
            </div>

            <div class="carousel__item">
              <div class="carousel__item-inner image-box">
                <img 
                  data-flickity-lazyload-srcset="https://picsum.photos/640/480/?image=10 640w, https://picsum.photos/480/360/?image=10 480w"
                  sizes="(min-width: 480px) 640px, 480px"
                  data-flickity-lazyload-src="https://picsum.photos/640/480/?image=10"
                  alt=""
                >
              </div>
            </div>

          </Flickity>
        </div>
        

        <!-- text -->
        <div class="module">
          <p v-for="n in 5" :key="n">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo similique ad reprehenderit laudantium necessitatibus alias, placeat provident, expedita aut autem laborum excepturi accusamus nesciunt culpa enim recusandae officia sunt quisquam. Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet numquam iste consequatur cupiditate placeat libero maiores animi odit exercitationem autem, cumque nisi excepturi obcaecati! Laboriosam ut voluptatem cum quibusdam? Aperiam! Lorem ipsum, dolor sit amet consectetur adipisicing elit. Iure voluptate soluta natus exercitationem aspernatur quo, laboriosam fugit debitis minima asperiores? Facilis ipsum nisi nam vel eveniet voluptatum ut obcaecati eligendi.
          </p>
        </div>

      </div>
    </main>

  </div>
</template>

<script>
  import Header from './components/Header';
  import Flickity from 'vue-flickity';

  export default {
    name: 'App',
    components: {
      Header,
      Flickity
    }
  }
</script>