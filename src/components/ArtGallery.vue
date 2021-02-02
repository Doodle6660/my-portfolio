<template>
    <div class="flex h-screen w-full hero">
        <div class="w-full items-center">
            <img src="@/assets/image/wave-art.svg" alt="" />
        </div>
    </div>
</template>

<script>
export default {}
</script>

<style scoped>
.hero {
    background: linear-gradient(
            135deg,
            rgba(32, 58, 67, 0.9) 0%,
            rgba(15, 32, 39, 0.8) 100%
        ),
        url("./../assets/image/art-bg.jpg") center no-repeat;
    background-size: cover;
}
</style>
