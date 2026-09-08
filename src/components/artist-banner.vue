<template>
  <div class="artist-banner">
    <div class="gradient-layer">
      <div class="artist-info">
        <h1 class="artist-pen-name">Mos'haf</h1>
        <h5 class="artist-name">Amir Mos'hafi</h5>
        <div class="artist-socials">
          <a href="https://www.youtube.com/moshafi/" target="_blank" rel="noopener noreferrer">
            <Icon icon="fa-brands:youtube" />
          </a>
          <a href="https://www.soundcloud.com/moshafi" target="_blank" rel="noopener noreferrer">
            <Icon icon="fa-brands:soundcloud" />
          </a>
          <a
            href="https://open.spotify.com/artist/0D5wNDVgW140e1H2893542"
            target="_blank"
            rel="noopener noreferrer"
          >
            <Icon icon="fa-brands:spotify" />
          </a>
        </div>
      </div>
    </div>
    <img src="../assets/images/artist-banner/banner.png" alt="Artist Banner" />
  </div>
</template>

<script setup lang="ts">
import { Icon } from '@iconify/vue'
</script>

<style scoped lang="scss">
.artist-banner {
  width: 100%;
  aspect-ratio: 1/1;
  overflow: hidden;
  position: relative;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  .gradient-layer {
    position: absolute;
    display: flex;
    justify-content: flex-end;
    align-items: flex-start;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(to bottom, rgba(0, 0, 0, 0), var(--bg-primary));

    z-index: 1;

    .artist-info {
      display: flex;
      flex-direction: column;
      justify-content: center;
      gap: 0.5rem;
      align-items: end;

      padding: 1rem;
      margin-top: 3rem;
      color: var(--text-primary);
      z-index: 2;

      .artist-pen-name {
        font-size: 4.5rem;
        font-family: var(--font-logo);
      }

      .artist-name {
        font-size: 0.8rem;
        font-weight: 400;
        letter-spacing: 0.25rem;
        color: var(--text-secondary);
        margin-left: 0.5rem;
      }

      .artist-socials {
        display: flex;
        gap: 1rem;
        margin-top: 1rem;
        margin-left: 0.5rem;

        a {
          color: var(--text-primary);
          font-size: 1.1rem;
          transition: color 0.3s ease;

          &:hover {
            color: var(--accent-color);
          }
        }
      }
    }
  }
}
</style>
