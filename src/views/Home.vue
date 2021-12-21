<template>
  <div class="home">
    <div class="home__header">
      <div><p class="slide-up yellow">Frontend</p></div>
      <div><p class="slide-up">development</p></div>
      <div><p class="slide-up">and inspired</p></div>
      <div><p class="slide-up blue">UI/UX design</p></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
};
</script>
<style>
.home {
  width: 100%;
  box-sizing: border-box;
  display: grid;
  grid-template-columns: repeat(7, 1fr);
  grid-template-rows: repeat(7, 1fr);
  grid-gap: 1rem;
  background-image: url(../assets/author.jpg);
  background-size: 70%;
  background-repeat: no-repeat;
  background-position: 160% -140%;
}

.home__header {
  font-family: 'Syne', sans-serif;
  font-size: 15.5vh;
  line-height: 1;
  grid-column: 1 / 7;
  grid-row: 3 / 7;
}

.home__header > div {
  cursor: default;
  overflow: hidden;
}

.home__header > div:nth-child(2) > p {
  -webkit-animation-delay: 0.1s;
  animation-delay: 0.1s;
}

.home__header > div:nth-child(3) > p {
  -webkit-animation-delay: 0.15s;
  animation-delay: 0.15s;
}

.home__header > div:nth-child(4) > p {
  -webkit-animation-delay: 0.2s;
  animation-delay: 0.2s;
}

.slide-up {
  -webkit-animation: slide-up 0.9s cubic-bezier(0.65, 0, 0.35, 1) both;
  animation: slide-up 0.9s cubic-bezier(0.65, 0, 0.35, 1) both;
}

.yellow {
  color: #FFBD00;
}

.blue {
  color: #2C6FF3;
}

@keyframes slide-up {
  0% {
    transform: translateY(150px);
  }
  100% {
    transform: translateY(0);
  }
}

@media screen and (max-width: 500px) {
  .home {
    background-position: bottom;
    background-size: 180%;
    grid-template-columns: repeat(7, 1fr);
    grid-template-rows: repeat(7, 1fr);
  }

  .home__header {
    grid-column: 1 / 8;
    grid-row: 1 / 4;
    font-size: 10vw;
    margin-left: 1rem;
  }
}
</style>
