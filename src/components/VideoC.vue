<template>
  <div class="banner">
    <div class="banner-bg"></div>
    <video class="d-none d-md-block" autoplay muted loop>
      <source src="@/assets/video-1.mp4" type="video/mp4">
    </video>
    <video class="d-md-none" autoplay muted loop>
      <source src="@/assets/video-mobile.mp4" type="video/mp4">
    </video>
    <div class="banner-text px-4 py-3 position-absolute translate-middle text-white fw-bold lh-base start-50 top-50 opacity-75 text-center">
      <h2 class="py-2">反抗瀕臨絕種<br>
      讓美麗的物種都能有活下去的機會</h2>
      <button type="button" class="btn btn-secondary">
        幫人類擦屁股
        <font-awesome-icon icon="fa-solid fa-toilet-paper"/>
      </button>
    </div>
  </div>
</template>

<style>

.banner{
  width: 100%;
  height: 100vh;
  overflow: hidden;
}

.banner-bg {
  position: absolute;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
  background: rgba(0,0,0, 0.2);
  z-index: -1;
}

.banner video{
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  object-fit: cover;
}

@media (min-width: 768px) {
  .banner-text {
    left: 20%;
  }
}

</style>
