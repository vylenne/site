<template>
  <div class="works">
    <div class="works__header">
      <div><p class="slide-up">There are no works here yet.</p></div>
      <div><p class="slide-up">They will be added later.</p></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Works',
};
</script>

<style scoped>
.works {
  width: 100%;
  box-sizing: border-box;
  display: grid;
  grid-template-columns: repeat(7, 1fr);
  grid-template-rows: repeat(7, 1fr);
  grid-gap: 1rem;
  position: relative;
}

.works__header {
  font-family: 'Syne', sans-serif;
  font-size: 7vh;
  line-height: 1;
  grid-column: 1 / 7;
  grid-row: 4;
}

.slide-up {
  -webkit-animation: slide-up 0.9s cubic-bezier(0.65, 0, 0.35, 1) both;
  animation: slide-up 0.9s cubic-bezier(0.65, 0, 0.35, 1) both;
}

.works__header > div {
  cursor: default;
  overflow: hidden;
}

.works__header > div:nth-child(2) > p {
  -webkit-animation-delay: 0.05s;
  animation-delay: 0.05s;
}
</style>
