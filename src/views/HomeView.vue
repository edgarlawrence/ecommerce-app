<template>
  <div id="home">
<div class="flex justify-center p-10 bg-sky-400 w-full">
    <!-- Carousel -->
    <div id="carouselExampleCaptions" class="carousel slide relative w-6/12" data-bs-ride="carousel">
      <div class="carousel-indicators absolute right-0 bottom-0 left-0 flex justify-center p-0 mb-4">
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="0"
          class="active"
          aria-current="true"
          aria-label="Slide 1"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="1"
          aria-label="Slide 2"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="2"
          aria-label="Slide 3"
        ></button>
      </div>
      <div class="carousel-inner relative w-full overflow-hidden">
        <div class="carousel-item active relative float-left w-full">
          <img
            src="https://mdbootstrap.com/img/Photos/Slides/img%20(15).jpg"
            class="block w-full"
            alt="..."
          />
          <div class="carousel-caption hidden md:block absolute text-center">
            <h5 class="text-xl">First slide label</h5>
            <p>Some representative placeholder content for the first slide.</p>
          </div>
        </div>
        <div class="carousel-item relative float-left w-full">
          <img
            src="https://mdbootstrap.com/img/Photos/Slides/img%20(22).jpg"
            class="block w-full"
            alt="..."
          />
          <div class="carousel-caption hidden md:block absolute text-center">
            <h5 class="text-xl">Second slide label</h5>
            <p>Some representative placeholder content for the second slide.</p>
          </div>
        </div>
        <div class="carousel-item relative float-left w-full">
          <img
            src="https://mdbootstrap.com/img/Photos/Slides/img%20(23).jpg"
            class="block w-full"
            alt="..."
          />
          <div class="carousel-caption hidden md:block absolute text-center">
            <h5 class="text-xl">Third slide label</h5>
            <p>Some representative placeholder content for the third slide.</p>
          </div>
        </div>
      </div>
      <button
        class="carousel-control-prev absolute top-0 bottom-0 flex items-center justify-center p-0 text-center border-0 hover:outline-none hover:no-underline focus:outline-none focus:no-underline left-0"
        type="button"
        data-bs-target="#carouselExampleCaptions"
        data-bs-slide="prev"
      >
        <span class="carousel-control-prev-icon inline-block bg-no-repeat" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button
        class="carousel-control-next absolute top-0 bottom-0 flex items-center justify-center p-0 text-center border-0 hover:outline-none hover:no-underline focus:outline-none focus:no-underline right-0"
        type="button"
        data-bs-target="#carouselExampleCaptions"
        data-bs-slide="next"
      >
        <span class="carousel-control-next-icon inline-block bg-no-repeat" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
  <!-- End of Carousel -->
</div>

  <!-- category section -->
    <div class="category">
      <div v-for="(item, index) in categories" :key="index">
        <div class="category-card">
            <img :src="item.img" />
            <h4> {{item.name}} </h4>
        </div>
      </div>
    </div>
  <!-- end of category section -->

  <!-- product with banner section -->
  <productList />
  <!-- end of product with banner section -->
      <productBanners :banners="banners"/>

  <!-- logo section -->
  <div class="homepage-logos">
    <div v-for="item in services" :key="item.id">
      <div class="homepage-logos-box">
        <img :src="item.img" alt="">  
        <h4 class="pt-5 font-bold"> {{item.title}} </h4>      
      </div>
    </div>
  </div>
  <!-- end of logo section -->

  <!-- about us -->
    <div class="about-us flex justify-center bg-sky-400 w-full p-20">
        <div class="about-us-images">
          <img :src="aboutUsimg" alt="">
        </div>
        <div class="pl-5 pr-5"></div>
        <div class="about-us-desc text-white">
          <h3 class="text-3xl font-bold">Tentang Kami</h3> <br>
          <p class="text-lg">
          Buildozzer merupakan situs belanja online terpercaya di Indonesia yang menjual beragam produk bangunan yang dibutuhkan masyarakat Indonesia.
          Seiring berkembangnya teknologi, semakin banyak aktivitas yang dilakukan secara digital, lebih mudah dan praktis, termasuk kegiatan pembelanjaan yang kini semakin marak dilakukan secara digital, baik melalui komputer, laptop, hingga smartphone yang bisa diakses kapan saja dan di mana saja.
          Kami hadir sebagai toko online terpercaya hal ini memungkinkan setiap orang untuk menjual dan juga membeli produk dengan mudah secara online. Setiap orang dapat memasarkan produk unggulannya di Buildozzer dengan membuka toko online murah dengan pilihan sistem belanja satuan dan juga grosir.
          </p>
        </div>
    </div>
  <!-- end of about us -->
  
  </div>
</template>



<style lang="scss">
#home {
  display: flex;
  flex-direction: column;
  align-items: center;

  .category {
    display: flex;
    justify-content: space-around;
    flex: 0;
    padding-top: 3rem;
    padding-bottom: 3rem;

    &-card {
      display: flex;
      justify-content: center;
      box-shadow: 0 8px 16px 0 rgb(0 0 0 / 20%);
      border-radius: 10px;
      margin: 1rem;
      width: 25rem;
      height: 7rem;
      padding-left: 4rem;
      padding-right: 4rem;
      align-items: center;
    }
  }

  .homepage-logos {
    display: flex;
    padding-top: 2rem;
    padding-bottom: 2rem;

    &-box {
      border: 1px solid #E5E5E5;
      padding: 2rem;
      margin: 1rem;
    }

    &-box img {
      width: 10rem;
    }
  }

  .about-us {
    &-desc {
      width: 42rem;
      text-align: left;
    }
  }
}
</style>

<script>
import img1 from '../images/category1.png'
import img2 from '../images/category2.png'
import img3 from '../images/category3.png'
import banner1 from '../images/cat.jpeg'
import banner2 from '../images/category-hand.png'
import banner3 from '../images/category-material.png'
import aboutUsimg from '../images/about-us.png'

import serviceImg1 from '../images/service1.png'
import serviceImg2 from '../images/service2.png'
import serviceImg3 from '../images/service3.png'
import serviceImg4 from '../images/service4.png'

import productList from '../components/product-list.vue'
import productBanners from '../components/product-banner.vue'

export default {
  name: 'HomeView',
  data() {
    return {
      categories:[
        {
          id: 1,
          name: "Alat Tukang",
          img: img1
        },
        {
          id: 2,
          name: "Cat",
          img: img2
        },
        {
          id: 3,
          name: "Platforn",
          img: img3
        }
      ],
      banners:[
        {
          id: 1,
          img: banner1,
          title: "Cat Perlengkapan"
        },
        {
          id: 2,
          img: banner2,
          title: "Alat Tukang"
        },
        {
          id: 3,
          img: banner3,
          title: "Material dan Bangunan"
        }
      ],
      services:[
        {
          id: 1,
          img: serviceImg1,
          title: "Pilihan Lengkap"
        },
        {
          id: 2,
          img: serviceImg2,
           title: "Produk Berkualitas"
        },
        {
          id: 3,
          img: serviceImg3,
           title: "Pelayanan Cepat"
        },
        {
          id: 4,
          img: serviceImg4,
           title: "Transaksi Aman"
        }
      ],
      aboutUsimg
    }
  },
  components: {
     productList,
     productBanners
  }
}
</script>
