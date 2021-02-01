<template>
    <div class="home">
        <app-home></app-home>
        <app-links></app-links>
        <app-bio></app-bio>
    </div>
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue"
import QuickLinks from "@/components/QuickLinks.vue"
import Biography from "@/components/Biography.vue"

export default {
    components: {
        "app-home": HelloWorld,
        "app-links": QuickLinks,
        "app-bio": Biography,
    },
}
</script>
