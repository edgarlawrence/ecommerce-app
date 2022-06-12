<template>
    <div id="ProductDetails">
        <div class="containers pt-20 pb-20">
            <div class="product-imgs">
                <img :src="ImgProduct" alt="">
            </div>
            <div class="product-desc">
                <div class="product-desc-header">
                    <h1 class="text-3xl"> Pompa Air </h1>
                </div>
                <div class="product-desc-option">
                    <div class="product-desc-option-variant pt-5">
                        <h1> Pilih Variant Anda </h1>
                        <div class="flex">
                            <div v-for="item in variants" :key="item.id">
                                <div class="rounded-full px-5 py-2 bg-sky-400 text-white m-1">
                                <p> {{item.text}}</p>
                                </div>
                            </div>
                    </div>

                    <div class="product-desc-option-deliver pt-5">
                        <h1> Pilih Variant Anda </h1>
                        <div class="flex">
                            <div v-for="item in deliveries" :key="item.id">
                                <div class="rounded-full px-5 py-2 bg-sky-400 text-white m-1">
                                <p> {{item.text}}</p>
                                </div>
                            </div>
                        </div> 
                    </div>   

                    <div class="product-desc-option-total pt-5">
                        <h1> Jumlah Pembelian </h1>
                        <div class="flex justify-between w-32 pt-3">
                            <button @click="decrementValue"> - </button>
                            <span class="counter-box"> {{ counter }} </span>
                            <button @click="incrementValue"> + </button>
                        </div> 
                    </div>  
                    </div>
                </div>

                <div class="product-payment pt-10">
                    <div class="product-payment-cta1 bg-gray-400 px-7 py-3 text-white rounded-lg">
                        <span> Add To Cart</span>
                    </div>
                    <div class="product-payment-cta2 bg-sky-400 px-7 py-3 text-white rounded-lg">
                        <span> Buy Now</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
#ProductDetails {
    .containers {
        display: flex;
        justify-content: center;
    }

    .product {
        &-imgs img {
            width: 25rem;
        }

        &-desc {
            text-align: left;
            margin-left: 2rem;
        }

        &-payment {
            display: flex;
            justify-content: space-between;
        }
    }

    .counter-box {
        background-color: rgb(56 189 248);
        padding: 1rem;
        border-radius: 10px;
        color: white;
    }
}
</style>

<script>
import ImgProduct from '../images/pompa-air.jpg'

export default {
    data() {
        return {
            variants: [
                {
                    id: 1,
                    text: "Kecil"
                },
                {
                    id: 2,
                    text: "Sedang"
                },
                {
                    id: 3,
                    text: "Besar"
                }
            ],
            deliveries: [
                {
                    id: 1,
                    text: "Reguler"
                },
                {
                    id: 2,
                    text: "Kilat"
                }
            ],
            ImgProduct,
            counter: 0
        }
    },
    methods: {
        incrementValue() {
        this.counter++;
        },
        decrementValue() {
        this.counter--;
            if (this.counter < 0) {
                this.counter = 0
            }
        },
        resetValue() {
        this.counter = 0;
        },
        logName: function(){
        console.log('firstName:', this.firstName);
        }
    }    
}
</script>
