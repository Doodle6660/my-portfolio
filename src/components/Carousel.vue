<template>
    <div class="flex flex-col w-full items-center">
        <div class="flex flex-row w-full md:w-3/5">
            <div class="flex w-1/2 justify-start">
                <p
                    class="text-2xl md:text-4xl xl:text-5xl font-semibold font-secondary"
                >
                    Project Works
                </p>
            </div>
            <div class="flex w-1/2 justify-end gap-x-3 md:gap-x-5">
                <button
                    @click="prev"
                    class="bg-moon1 px-2 py-2 md:px-3 md:py-3 rounded-lg focus:outline-none active:bg-moon2"
                >
                    <svg
                        xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 24 24"
                        fill="none"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        class="w-6 h-6 stroke-2 stroke-current text-white"
                    >
                        <path d="M11 17l-5-5 5-5M18 17l-5-5 5-5" />
                    </svg>
                </button>
                <button
                    @click="next"
                    class="bg-moon1 px-2 py-2 md:px-3 md:py-3 rounded-md focus:outline-none active:bg-moon2"
                >
                    <svg
                        xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 24 24"
                        fill="none"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        class="w-6 h-6 stroke-2 stroke-current text-white"
                    >
                        <path d="M13 17l5-5-5-5M6 17l5-5-5-5" />
                    </svg>
                </button>
            </div>
        </div>
        <div
            class="carousel focus:outline-none"
            @keydown="checkSlide($event)"
            tabindex="0"
        >
            <slot></slot>
        </div>
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

<style scoped></style>
