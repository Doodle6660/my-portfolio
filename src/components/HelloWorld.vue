<template>
    <div class="flex flex-row h-screen  text-white hello">
        <div
            class="flex flex-col max-w-xl h-full items-start justify-center ml-6 xl:ml-12 font-primary z-50"
        >
            <div
                class="text-6xl md:text-7xl xl:text-8xl leading-snug md:leading-snug font-bold"
            >
                <p>Hello.</p>
                <p>Im Ziyad</p>
            </div>
            <div class="text-3xl xl:text-5xl mt-8">
                <p class="p2">Front-End & UI/UX Designer</p>
            </div>
            <div class="text-md xl:text-2xl mt-32 md:mt-20 font-secondary z-50">
                <p class="p3">
                    Hi!
                    <span class="font-semibold">I'm an 18-year-old maker</span>
                    who enjoys building simple & clean websites that are easy to
                    use and beautiful to look at.
                </p>
            </div>
        </div>

        <div class="hidden md:flex items-end justify-center w-full h-full z-50">
            <img
                src="./../assets/image/avatar.png"
                class="avatar-image md:w-80 xl:w-96"
            />
        </div>

        <app-bubble></app-bubble>
    </div>
</template>

<script>
import Bubble from "@/components/Bubble.vue"

export default {
    components: {
        "app-bubble": Bubble,
    },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
    background: url("./../assets/image/nature2.jpg") center no-repeat;
    background-size: cover;
}

p {
    text-shadow: 4px 4px rgba(0, 0, 0, 0.5);
}

.p2 {
    text-shadow: 3px 3px rgba(0, 0, 0, 0.5);
}

.p3 {
    text-shadow: 2px 2px rgba(0, 0, 0, 0.5);
}
</style>
