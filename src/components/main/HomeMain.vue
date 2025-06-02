<script>
export default {
  name: "HomeMain",
};
</script>

<template>
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-12 col-lg-6">
        <p class="display-5 text-center text-lg-start">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Incidunt ad
          excepturi molestiae debitis nesciunt labore veniam, et iste. Autem
          cupiditate in nulla doloremque consectetur, ipsa dolor fugit vitae
          facilis eligendi.
        </p>
      </div>
      <div class="col-12 col-lg-6">
        <img src="../../assets/img/home/3_hand.png" alt="" />
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-12 col-lg-6">
        <p class="display-5 text-center text-lg-start">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Incidunt ad
          excepturi molestiae debitis nesciunt labore veniam, et iste. Autem
          cupiditate in nulla doloremque consectetur, ipsa dolor fugit vitae
          facilis eligendi.
        </p>
      </div>
      <div class="col-12 col-lg-6">
        <img src="../../assets/img/home/3_hand.png" alt="" />
      </div>
    </div>
  </div>
</template>

<style scoped>
img {
  width: 90%;
}

.keyword-slider {
  overflow-x: none;
  white-space: nowrap;
}

.scrolling-keywords {
  display: inline-block;
  animation: scroll 30s linear infinite;
}

@keyframes scroll {
  0% {
    transform: translateX(100%);
  }

  100% {
    transform: translateX(-100%);
  }
}
</style>
