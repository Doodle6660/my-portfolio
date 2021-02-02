<template>
    <div class="carousel" @keydown="checkSlide($event)" tabindex="0">
        <slot></slot>
        <button @click="next" class="btn btn-next">Next</button>
        <button @click="prev" class="btn btn-prev">Prev</button>
    </div>
</template>

<script>
export default {
    data() {
        return {}
    },
    methods: {
        next() {
            this.$emit("next")
        },
        prev() {
            this.$emit("prev")
        },
    },
}
</script>

<style>
.carousel {
    position: relative;
    width: 600px;
    height: 350px;
    overflow: hidden;
}
</style>
