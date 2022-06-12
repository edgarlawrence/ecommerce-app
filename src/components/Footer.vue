<template>
    <div id="footers" class="bg-gray-300">
        <div class="info1 text-left">
            <ul>
                <h1 class="text-3xl pb-5">Alamat Kami</h1>
                <p class="w-60">
                    Jl. Sidorukun No. 121 A-B
                    Medan - Sumatera Utara
                    20239
                    Email	:	pt.grahapilarbangunan_bison@yahoo.com
                    contact@buildozzer.co.id
                    Customer Service : (061) 800-3333-5 / 800-3333-6
                </p>
            </ul>
        </div>
        <div class="info2 text-left">
            <ul>
                <h1 class="text-3xl pb-5">Cara belanja</h1>
                <li class="p-1"> Pembayaran yang kami terima </li>
                <li class="p-1"> Konfirmasi pembayaran </li>
                <li class="p-1"> FAQ </li>
                <li class="p-1"> Syarat dan ketentuan </li>
                <li class="p-1"> Kontak kami </li>
                <li class="p-1"> Kebijakan Privasi </li>
            </ul>
        </div>
        <div class="logo">
            <h1 class="text-3xl text-left pb-5">Unduh Kami Di</h1>
            <div class=" inline-flex">
                <img :src="appstore" alt="">
                <div class="pl-3 pr-3">

                </div>
                <img :src="gplay" alt="">
            </div>
        </div>
    </div>
</template>

<style lang="scss">
    #footers {
        display: flex;
        justify-content: center;
        justify-content: space-around;
        padding-top: 2rem;
        padding-bottom: 2rem;

        .logo img {
            height: 3rem;
        }
    }
</style>

<script>
import appstore from '../images/apstore.png';
import gplay from '../images/gplay.png';

export default {
    name: 'Footer',
    data() {
        return {
            appstore, gplay
        }
    }
}
</script>