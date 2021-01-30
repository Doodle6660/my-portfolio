<template>
    <div
        class="flex flex-row h-screen bg-gradient-to-r from-black to-primary text-white"
    >
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
                <p>Front-End & UI/UX Designer</p>
            </div>
            <div class="text-md xl:text-2xl mt-32 md:mt-20 font-secondary z-50">
                <p>
                    Hi!
                    <span class="font-semibold">I'm an 18-year-old maker</span>
                    who enjoys building simple & clean websites that are easy to
                    use and beautiful to look at.
                </p>
            </div>
        </div>

        <div class="hidden md:flex items-end justify-center w-full h-full z-50">
            <img src="./../assets/image/avatar.png" class="avatar-image w-96" />
        </div>

        <div class="bubbles z-10">
            <div class="bubble z-10"></div>
            <div class="bubble z-10"></div>
            <div class="bubble z-10"></div>
            <div class="bubble z-10"></div>
            <div class="bubble z-10"></div>
            <div class="bubble z-10"></div>
            <div class="bubble z-10"></div>
            <div class="bubble z-10"></div>
            <div class="bubble z-10"></div>
            <div class="bubble z-10"></div>
        </div>
    </div>
</template>

<script></script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bubbles {
    position: absolute;
    width: 100%;
    height: 100%;
    z-index: 0;
    overflow: hidden;
    top: 0;
    left: 0;
}
.bubble {
    position: absolute;
    bottom: -100px;
    width: 10px;
    height: 10px;
    background: #f1f1f1;
    border-radius: 50%;
    animation: rise 5s infinite ease-in;
}
.bubble:nth-child(1) {
    width: 20px;
    height: 20px;
    left: 10%;
    animation-duration: 8s;
}
.bubble:nth-child(2) {
    width: 10px;
    height: 10px;
    left: 20%;
    animation-duration: 5s;
    animation-delay: 1s;
}
.bubble:nth-child(3) {
    width: 10px;
    height: 10px;
    left: 35%;
    animation-duration: 7s;
    animation-delay: 2s;
}
.bubble:nth-child(4) {
    width: 10px;
    height: 10px;
    left: 50%;
    animation-duration: 11s;
    animation-delay: 0s;
}
.bubble:nth-child(5) {
    width: 20px;
    height: 20px;
    left: 55%;
    animation-duration: 6s;
    animation-delay: 1s;
}
.bubble:nth-child(6) {
    width: 10px;
    height: 10px;
    left: 65%;
    animation-duration: 8s;
    animation-delay: 3s;
}
.bubble:nth-child(7) {
    width: 10px;
    height: 10px;
    left: 70%;
    animation-duration: 12s;
    animation-delay: 2s;
}
.bubble:nth-child(8) {
    width: 10px;
    height: 10px;
    left: 80%;
    animation-duration: 6s;
    animation-delay: 2s;
}
.bubble:nth-child(9) {
    width: 10px;
    height: 10px;
    left: 70%;
    animation-duration: 5s;
    animation-delay: 1s;
}
.bubble:nth-child(10) {
    width: 10px;
    height: 10px;
    left: 25%;
    animation-duration: 10s;
    animation-delay: 4s;
}
@keyframes rise {
    0% {
        bottom: -100px;
        transform: translateX(0);
    }
    50% {
        transform: translate(100px);
    }
    100% {
        bottom: 1080px;
        transform: translateX(-200px);
    }
}
</style>
