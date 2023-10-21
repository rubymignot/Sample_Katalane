<template>
    <nav class="header__nav">
        <div class="flex flex-wrap items-center justify-between mx-auto p-2 bg-black/40">
            <div class="navbar">
                <div class="navbar-start">
                    <div class="dropdown">
                        <label tabindex="0" class="btn btn-ghost md:hidden">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24"
                                stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                    d="M4 6h16M4 12h8m-8 6h16" />
                            </svg>
                        </label>
                        <ul tabindex="0"
                            class="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow bg-base-100 rounded-box w-52">
                            
                        <template v-for="item in menuItems" :key="item.name">
                            <li>
                                <NuxtLink :to="item.link">{{ item.name }}</NuxtLink>
                            </li>
                        </template>
                        </ul>
                    </div>
                </div>
                <div class="navbar-center hidden md:flex">
                    <ul id="menu-md" class="menu menu-horizontal px-1">
                        <template v-for="item in menuItems" :key="item.name">
                            <li>
                                <NuxtLink :to="item.link">{{ item.name }}</NuxtLink>
                            </li>
                        </template>
                    </ul>
                </div>
                <div class="navbar-end">
                </div>
            </div>
        </div>
    </nav>
</template>
<script setup lang="ts">
const menuItems = [
    { name: 'HOME', link: '/' },
    { name: 'OUR FLOAT', link: '#' },
    { name: 'KATALANE NETWORK', link: '#' },
    { name: 'BOAT SHOWS', link: '#' },
    { name: 'NEWS', link: '#' },
    { name: 'CONTACT', link: '#' },
]
</script>