<template>
    <div class="home">
        <app-home></app-home>
        <app-links></app-links>
        <app-bio></app-bio>
        <app-project></app-project>
        <app-art></app-art>
    </div>
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue"
import QuickLinks from "@/components/QuickLinks.vue"
import Biography from "@/components/Biography.vue"
import Project from "@/components/Project.vue"
import ArtWork from "@/components/ArtGallery.vue"

export default {
    components: {
        "app-home": HelloWorld,
        "app-links": QuickLinks,
        "app-bio": Biography,
        "app-project": Project,
        "app-art": ArtWork,
    },
}
</script>
