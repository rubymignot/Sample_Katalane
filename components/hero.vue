<template>
    <section class="hero__img flex min-h-screen">
        <div class="header">
            <div class="alert rounded-none py-2 bg-gray-200 text-black font-bold" v-if="alert_sample">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                    class="stroke-current shrink-0 w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                </svg>
                <span>This is a sample/demo website, most links won't work. To visit my portfolio, go to <a
                        class="link link-hover" href="https://rubymignot.com">rubymignot.com</a></span>
                <div>
                    <button class="btn btn-sm" @click="close_alert">Close</button>
                </div>
            </div>
            <div class="header__logo p-4 bg-white">
                <img class="h-full"
                    src="https://res.cloudinary.com/dfoesshfi/image/upload/f_auto,q_auto/v1/Katalane/aat0gpulqfnpicb3nhk4"
                    alt="Katalane Logo" />
                <h1 class="hidden sm:flex">Katalane</h1>
            </div>
            <Navigation></Navigation>
            <div class="hero__index">
                <div class="flex flex-col gap-5">
                    <h1 class="text-4xl text-white font-bold">Set Sail Beyond the Horizon</h1>
                    <a class="btn bg-blue-500 text-white rounded-none border-none" href="#">Discover Our Fleet</a>
                </div>
                <HeroForm></HeroForm>
            </div>
        </div>
        <div class="w-full absolute h-full bg-black/30"></div>
    </section>
</template>
<script setup lang="ts">
const alert_sample = ref(true)
// turn off alert_sample to remove the alert
async function close_alert() {
    alert_sample.value = false
}
</script>