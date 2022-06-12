<template>
    <div id="sign-up">
        <form class="w-full max-w-lg">
        <div class="form-header py-10 text-3xl">
            <h1> Daftar Akun </h1>
        </div>
        <div class="flex flex-wrap -mx-3 mb-6">
            <div class="w-full px-3 mb-6 md:mb-0">
            <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-first-name">
                Nama Lengkap
            </label>
            <input class="appearance-none block w-full bg-gray-200 text-gray-700 border rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white" id="grid-first-name" type="text">
            <!-- <p class="text-red-500 text-xs italic">Please fill out this field.</p> -->
            </div>
        </div>
        <div class="flex flex-wrap -mx-3 mb-6">
            <div class="w-full px-3 mb-6 md:mb-0">
            <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-first-name">
                Email
            </label>
            <input class="appearance-none block w-full bg-gray-200 text-gray-700 border rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white" id="grid-first-name" type="email">
            <!-- <p class="text-red-500 text-xs italic">Please fill out this field.</p> -->
            </div>
        </div>
        <div class="flex flex-wrap -mx-3 mb-6">
            <div class="w-full md:w-1/2 px-3 mb-6 md:mb-0">
            <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-first-name">
                Nomor Telepon
            </label>
            <input class="appearance-none block w-full bg-gray-200 text-gray-700 border rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white" id="grid-first-name" type="number">
            <!-- <p class="text-red-500 text-xs italic">Please fill out this field.</p> -->
            </div>
            <div class="w-full md:w-1/2 px-3">
            <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-last-name">
                Tanggal Lahir
            </label>
            <input class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500" id="grid-last-name" type="date">
            </div>
        </div>
        <div class="flex justify-center pb-7">
            <div class="w-full px-3 mb-6 md:mb-0">
                        <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-first-name">
                            Jenis Kelamin
                        </label>
                <select class="form-select appearance-none
                block
                w-full
                px-3
                py-1.5
                text-base
                font-normal
                text-gray-700
                bg-white bg-clip-padding bg-no-repeat
                border border-solid border-gray-300
                rounded
                transition
                ease-in-out
                m-0
                focus:text-gray-700 focus:bg-white focus:border-blue-600 focus:outline-none" aria-label="Default select example">
                    <option selected>Pilih Jenis Kelamin anda</option>
                    <option value="1">Laki-Laki</option>
                    <option value="2">Perempuan</option>
                </select>
            </div>
        </div>
        <div class="flex flex-wrap -mx-3 mb-6">
            <div class="w-full px-3">
            <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-password">
                Kata Sandi
            </label>
            <input class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500" id="grid-password" type="password" placeholder="******************">
            <!-- <p class="text-gray-600 text-xs italic">Make it as long and as crazy as you'd like</p> -->
            </div>
        </div>
        <div class="flex flex-wrap -mx-3 mb-6">
            <div class="w-full px-3">
            <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-password">
                Konfirmasi Kata Sandi
            </label>
            <input class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500" id="grid-password" type="password" placeholder="******************">
            <!-- <p class="text-gray-600 text-xs italic">Make it as long and as crazy as you'd like</p> -->
            </div>
        </div>
        <div class="md:flex mb-6">
            <div class="md:w-2/12"></div>
            <label class="md:w-2/3 block text-gray-500 font-bold">
            <input class="mr-2 leading-tight" type="checkbox">
            <span class="text-sm">
                Send me your newsletter!
            </span>
            </label>
        </div>
        <div class="sign-up">
            <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline" type="button">
                Daftar
            </button>
        </div>
        </form>
    </div>
</template>

<style lang="scss">
#sign-up {
    display: flex;
    justify-content: center;
    padding-top: 3rem;
    padding-bottom: 3rem;
}
</style>

<script>
import { Menu, MenuButton, MenuItem, MenuItems } from '@headlessui/vue'
import { ChevronDownIcon } from '@heroicons/vue/solid'

export default {
    
}
</script>