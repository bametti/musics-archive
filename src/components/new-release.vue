<template>
  <div class="new-release">
    <div class="wrapper">
      <div class="music-cover">
        <img src="../assets/images/music-cover/faghat-naro.jpg" alt="Faghat Naro" />
      </div>
      <div class="music-info">
        <span class="badge">NEW RELEASE</span>
        <div class="info">
          <h4 class="music-name">Faghat Naro</h4>
          <p class="artist-name">Mos'haf</p>
        </div>
        <p class="music-time">3:45</p>
      </div>
      <div class="play-button">
        <button>
          <Icon icon="fa-solid:play" />
        </button>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { Icon } from '@iconify/vue'
</script>

<style lang="scss" scoped>
.new-release {
  .wrapper {
    display: flex;
    height: 110px;
    flex-direction: row-reverse;
    align-items: center;
    justify-content: space-between;
    padding: 1rem;
    background-color: var(--bg-secondary);
    border-radius: 1rem;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);

    .music-cover {
      width: 25%;

      overflow: hidden;
      border-radius: 0.5rem;

      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }

    .music-info {
      display: flex;
      flex-direction: column;
      width: 65%;
      text-align: left;
      padding-left: 1rem;
      gap: 0.5rem;

      .badge {
        font-size: 0.65rem;
        color: var(--accent-dark);
      }
      .info {
        display: flex;
        flex-direction: column;
        gap: 0.25rem;

        .music-name {
          font-size: 1.1rem;
          font-weight: bold;
        }
        .artist-name {
          font-size: 0.75rem;
          color: var(--text-secondary);
        }
      }
      .music-time {
        font-size: 0.75rem;
        color: var(--text-secondary);
      }
    }

    .play-button {
      width: 10%;
      height: 100%;
      display: flex;
      align-items: flex-end;

      button {
        border-radius: 50%;
        border: none;
        display: flex;
        align-items: center;
        justify-content: center;
        width: 35px;
        height: 35px;
        opacity: 0.6;

        i {
          font-size: 0.2rem;
        }
      }
    }
  }
}
</style>
