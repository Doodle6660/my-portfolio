<template>
    <transition :name="direction">
        <div v-show="visibleSlide === index" class="carousel-slide">
            <slot></slot>
        </div>
    </transition>
</template>

<script>
export default {
    props: ["visibleSlide", "index", "direction"],
    data() {
        return {}
    },
}
</script>

<style scoped>
.left-enter-active {
    animation: leftInAnimation 0.5s ease-in-out;
}
.left-leave-active {
    animation: leftOutAnimation 0.5s ease-in-out;
}
@keyframes leftInAnimation {
    from {
        transform: translateX(100%);
    }
    to {
        transform: translateX(0%);
    }
}
@keyframes leftOutAnimation {
    from {
        transform: translateX(0%);
    }
    to {
        transform: translateX(-100%);
    }
}

.right-enter-active {
    animation: rightInAnimation 0.5s ease-in-out;
}
.right-leave-active {
    animation: rightOutAnimation 0.5s ease-in-out;
}
@keyframes rightInAnimation {
    from {
        transform: translateX(-100%);
    }
    to {
        transform: translateX(0%);
    }
}
@keyframes rightOutAnimation {
    from {
        transform: translateX(0%);
    }
    to {
        transform: translateX(100%);
    }
}
</style>
