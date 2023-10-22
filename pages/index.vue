<template>
    <Hero></Hero>
    <section class="section__paragraph">

        <h3 class="text-lg text-gray-500 py-4">Discover the Horizon with Katalane Catamarans</h3>
        <h2 class="text-2xl text-red-400">Sail. Explore. Thrive.</h2>
        <p class="text-gray-500 py-2">Embark on unforgettable voyages aboard Katalane's premier catamarans. Expertly crafted
            and designed for the adventurous soul, our vessels ensure safety, comfort, and a touch of luxury as you sail
            towards the next horizon. Dive into the world of Katalane and let the sea set you free.</p>
    </section>
    <section class="section__listing">
        <template v-for="image in Images">
            <a href="#">
                <div class="card w-full before:!rounded-none rounded-none shadow-xl image-full">
                    <figure><img class="w-full" :src="image.img" :alt="image.alt" /></figure>
                    <div class="card-body !text-white justify-end items-center bg-black/5 hover:bg-white/5">
                        <h3 class="card-title p-2 border-t border-white">{{ image.alt }}</h3>
                    </div>
                </div>
            </a></template>
    </section>
    <footer class="footer footer-center p-4 bg-base-300 text-base-content">
        <aside>
            <a href="https://rubymignot.com">© {{ new Date().getFullYear() }} Ruby Mignot, click here to access my website -
                Katalane is a fictional brand</a>
        </aside>
    </footer>
</template>
<script setup lang="ts">
const Images = [
    { img: "https://res.cloudinary.com/dfoesshfi/image/upload/f_auto,q_auto/v1/Katalane/Listing/maqdlqxb41hnv05jzz19", alt: "Latest Listings" },
    { img: "https://res.cloudinary.com/dfoesshfi/image/upload/f_auto,q_auto/v1/Katalane/Listing/zmbbi9cu41rroynjvomv", alt: "Latest Price Cuts" },
    { img: "https://res.cloudinary.com/dfoesshfi/image/upload/f_auto,q_auto/v1/Katalane/Listing/y5vad1vxcnsrgz7ndmwc", alt: "Most Visited Catamarans" }
]
</script>