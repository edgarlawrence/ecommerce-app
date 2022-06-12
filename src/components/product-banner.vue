<template>
    <div id="productBanners">
        <div v-for="item in banners" :key="item.id" class="banners pt-8">
            <div class="product-header flex items-center justify-between border-b-4 border-sky-400  pt-5 pb-5">
                <div class="title">
                    <h1 class="text-5xl"> {{item.title}} </h1>
                </div>
                <div class="buttons text-xl rounded-md bg-sky-400 p-5 text-white">
                    <a href="" class=""> Lihat Semua </a>
                </div>
            </div>
        <div class="containers">
            <div class="banner-img pt-10">
                <img :src="item.img" alt="">
            </div>
                <div v-for='index in 3' :key='index'>
                    <div class="w-60 rounded overflow-hidden shadow-lg m-10">
                    <img class="w-full" :src="barang1" alt="Sunset in the mountains">
                        <div class="px-6 py-4">
                            <div class="font-bold text-xl mb-2"> Besi Merah </div>
                                <p class="text-gray-700 text-base">
                                    Rp. 500.000
                                </p>
                                <p class="text-gray-700 text-xs pt-10">
                                    Toko Senang Jaya
                                </p>
                        </div>
                </div>
            </div>
        </div>
        </div>
    </div>
</template>

<style lang="scss">
#productBanners {
    .containers {
        display: grid;
        grid-template-columns: auto auto auto auto;
    }

    .banner-img img{
        width: 19rem;
    }
}
</style>

<script>
import barang1 from '../images/besi.webp'

export default {
    props:{
        banners: {
            type: Array
        }
    },
    data() {
        return {
            barang1
        }
    },
    mounted() {
        console.log(this.banner)
    }    
}
</script>