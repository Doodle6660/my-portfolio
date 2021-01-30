<template>
    <div class="home">
        <app-home></app-home>
        <app-links></app-links>
    </div>
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue"
import QuickLinks from "@/components/QuickLinks.vue"

export default {
    components: {
        "app-home": HelloWorld,
        "app-links": QuickLinks,
    },
}
</script>
