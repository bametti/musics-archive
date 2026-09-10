<template>
  <div class="home-page">
    <div class="top-side">
      <ArtistBanner class="artist-banner"></ArtistBanner>
      <NewRelease class="new-release"></NewRelease>
    </div>
  </div>
</template>

<script setup lang="ts">
import ArtistBanner from '@/components/artist-banner.vue'
import NewRelease from '@/components/new-release.vue'
</script>

<style scoped>
.top-side {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;

  .artist-banner {
    width: 100%;
    aspect-ratio: 1/1;
    overflow: hidden;
    position: relative;
  }

  .new-release {
    position: absolute;
    bottom: 0;
    width: 90%;
    z-index: 2;
  }
}
</style>
