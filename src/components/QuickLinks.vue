<template>
    <div class="flex flex-col w-full h-screen font-secondary">
        <div class="w-full items-center">
            <img src="@/assets/image/wave.svg" class="w-full" />
        </div>
        <div class="flex flex-col w-full h-full items-center justify-center">
            <p class="font-bold mb-10 text-2xl">Quick Links</p>
            <div
                class="flex flex-row w-full justify-between px-4 md:px-24 xl:px-52 text-base md:text-xl"
            >
                <a
                    href="#!"
                    class="text-red-400 font-semibold border-2 border-red-400 px-2 py-1 xl:px-4 xl:py-2 rounded-sm rounded-tl-2xl rounded-br-2xl duration-300 hover:bg-red-400 hover:text-white quick-btn"
                    >Biography</a
                >
                <a
                    href="#!"
                    class="text-blue-400 font-semibold border-2 border-blue-400 px-2 py-1 xl:px-4 xl:py-2 rounded-sm rounded-tl-2xl rounded-br-2xl duration-300 hover:bg-blue-400 hover:text-white quick-btn"
                    >Project Works</a
                >
                <a
                    href="#!"
                    class="text-green-400 font-semibold border-2 border-green-400 px-2 py-1 xl:px-4 xl:py-2 rounded-sm rounded-tl-2xl rounded-br-2xl duration-300 hover:bg-green-400 hover:text-white quick-btn"
                    >Art Works</a
                >
            </div>
        </div>

        <div class="flex flex-col w-full h-full justify-center">
            <p class="font-bold text-xl md:text-2xl items-start ml-3 md:ml-14">
                Experience :
            </p>
            <div
                class="flex flex-row w-full h-full justify-center space-x-6 md:space-x-20 xl:space-x-28"
            >
                <img
                    src="@/assets/image/vuejs.svg"
                    class="w-14 md:w-20 xl:w-24"
                />
                <img
                    src="@/assets/image/clipstudiopaint.svg"
                    class="w-14 md:w-20 xl:w-24"
                />
                <img
                    src="@/assets/image/figma.svg"
                    class="w-10 md:w-16 xl:w-20"
                />
                <img
                    src="@/assets/image/vuetify.svg"
                    class="w-10 md:w-20 xl:w-24"
                />
                <img
                    src="@/assets/image/firebase.svg"
                    class="w-10 md:w-20 xl:w-24"
                />
            </div>
            <a
                href="#!"
                class="text-center font-semibold text-red-400 font-primary mb-24 md:mb-8"
                >See More >></a
            >
        </div>
    </div>
</template>

<script>
export default {}
</script>

<style scoped>
.quick-btn:hover {
    border-top-right-radius: 1rem;
    border-bottom-left-radius: 1rem;
    border-top-left-radius: 0.125rem;
    border-bottom-right-radius: 0.125rem;
}
</style>
