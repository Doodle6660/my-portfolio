<template>
    <div
        class="flex h-screen w-full font-frimary justify-center px-4 md:px-0 footer"
    >
        <div class="flex flex-col justify-center items-center">
            <p class="text-xl md:text-5xl font-semibold mb-14">
                And that's me, in a nutshell.
            </p>
            <div
                class="flex flex-row w-full bg-moon1 px-4 md:px-8 py-8 text-white items-center rounded-xl"
            >
                <div class="w-3/5 md:w-3/4 flex-col text-xs md:text-sm">
                    <p class="text-lg md:text-2xl font-semibold mb-8 md:mb-14">
                        Work Inquiry
                    </p>
                    <p>
                        Let’s work together and I’ll help you by all my best :D
                    </p>
                </div>
                <div
                    class="w-2/5 md:w-1/4 bg-white px-1 md:px-2 py-2 md:py-4 text-moon1 text-center rounded-md"
                >
                    <a
                        href="#!"
                        class="uppercase font-semibold text-xs md:text-base"
                        >let's chat!</a
                    >
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {}
</script>

<style scoped>
.footer {
    background: linear-gradient(
            135deg,
            rgba(32, 58, 67, 0.2) 0%,
            rgba(15, 32, 39, 0.3) 100%
        ),
        url("./../assets/image/paper.jpg") center no-repeat;
    background-size: cover;
}
</style>
