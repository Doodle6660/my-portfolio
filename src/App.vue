<template>
    <router-view />
</template>

<script>
export default {
    components: {},
    data() {
        return {}
    },
    methods: {},
}
</script>

<style>
/* import fonts */
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&family=Quicksand:wght@300;400;500;600;700&display=swap");

::-webkit-scrollbar {
    width: 0.375rem;
    height: 6px;
}

::-webkit-scrollbar-track {
    box-shadow: inset 0 0 5px #000;
}

::-webkit-scrollbar-thumb {
    @apply bg-moon1;
    @apply rounded;
}

::-webkit-scrollbar-thumb:hover {
    @apply bg-moon3;
}
</style>
