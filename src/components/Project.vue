<template>
    <div class="flex h-screen w-full justify-center items-center">
        <app-carousel @next="next" @prev="prev">
            <app-carousel-slide
                v-for="(slide, index) in slides"
                :key="slide"
                :index="index"
                :visibleSlide="visibleSlide"
                :direction="direction"
                class="carousel-slider"
            >
                <img :src="slide" :alt="slide" />
            </app-carousel-slide>
        </app-carousel>
    </div>
</template>

<script>
import Carousel from "./Carousel.vue"
import CarouselSlide from "./CarouselSlide.vue"

export default {
    data() {
        return {
            slides: [
                "https://picsum.photos/id/230/600/300",
                "https://picsum.photos/id/231/600/300",
                "https://picsum.photos/id/232/600/300",
                "https://picsum.photos/id/233/600/300",
                "https://picsum.photos/id/234/600/300",
                "https://picsum.photos/id/235/600/300",
                "https://picsum.photos/id/236/600/300",
            ],
            visibleSlide: 0,
            direction: "",
        }
    },
    components: {
        "app-carousel": Carousel,
        "app-carousel-slide": CarouselSlide,
    },
    computed: {
        slidesLen() {
            return this.slides.length
        },
    },
    methods: {
        next() {
            if (this.visibleSlide >= this.slidesLen - 1) {
                this.visibleSlide = 0
            } else {
                this.visibleSlide++
            }
            this.direction = "left"
        },
        prev() {
            if (this.visibleSlide <= 0) {
                this.visibleSlide = this.slidesLen - 1
            } else {
                this.visibleSlide--
            }
            this.direction = "right"
        },
    },
}
</script>

<style>
.carousel {
    position: relative;
    overflow: hidden;
    width: 800px;
    height: 500px;
    z-index: 10;
}

.btn {
    padding: 5px 10px;
    background-color: rgba(0, 0, 0, 0.5);
    border: 1px solid transparent;
    margin: 5px 10px;
    color: #fff;
    height: 50px;
    width: 50px;
    position: absolute;
    margin-top: -25px;
    z-index: 2;
}
.btn:hover {
    cursor: pointer;
}

.btn:focus {
    outline: none;
}

.btn-next {
    top: 50%;
    right: 0;
}

.btn-prev {
    top: 50%;
    left: 0;
}

.carousel-slider {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
}

.carousel-slider img {
    width: 100%;
    height: 100%;
}
</style>
