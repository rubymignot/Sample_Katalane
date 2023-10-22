<template>
    <div class="hero__form">
                <form>
                    <div class="flex flex-col flex-wrap items-end">
                        <div class="flex flex-col w-full md:flex-row flex-wrap md:items-end gap-4">
                            <div class="mb-4">
                                <label class="block mb-2 text-sm font-medium" for="length">Boat Length Range:</label>
                                <input class="w-full p-2 bg-gray-50 border-gray-300 border-[1px]" type="text" id="length"
                                    placeholder="Min.">
                            </div>
                            <div class="mb-4">
                                <input class="w-full p-2 bg-gray-50 border-gray-300 border-[1px]" type="text" id="length"
                                    placeholder="Max.">
                            </div>
                        </div>
                        <div class="flex flex-col w-full md:flex-row flex-wrap md:items-end gap-4">
                            <div class="mb-4">
                                <label class="block mb-2 text-sm font-medium" for="length">Price Range (in €):</label>
                                <input class="w-full p-2 bg-gray-50 border-gray-300 border-[1px]" type="text" id="length"
                                    placeholder="From">
                            </div>
                            <div class="mb-4">
                                <input class="w-full p-2 bg-gray-50 border-gray-300 border-[1px]" type="text" id="length"
                                    placeholder="To">
                            </div>
                        </div>

                    </div>

                    <div class="mb-4">
                        <select class="w-full p-2 bg-gray-50 border-gray-300 border-[1px]" placeholder="From">
                            <option value="" disabled selected>Boat Type</option>
                            <option value="1">Catamaran</option>
                            <option value="2">Monohull</option>
                        </select>
                    </div>

                    <div class="mb-4">

                        <input class="w-full p-2 bg-gray-50 border-gray-300 border-[1px]" type="text" id="length"
                            placeholder="Location (eg. 123 Katalane Street)">
                    </div>


                    <div class="mb-4">

                        <input class="w-full p-2 bg-gray-50 border-gray-300 border-[1px]" type="text" id="length"
                            placeholder="Boat name">
                    </div>
                    <button class="btn rounded-none border-none bg-blue-500 text-white hover:bg-blue-600 w-full">
                        Search Catamarans
                    </button>
                </form>
            </div>
</template>