<template>
    <div class="home">
        <app-home></app-home>
    </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue"

export default {
    components: {
        "app-home": HelloWorld,
    },
}
</script>
