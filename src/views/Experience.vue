<template>
  <div class="experience">
    <div class="technologies">
      <p class="experience__header">Technologies I use</p>
      <div class="technologies__blocks">
        <div class="block">
          <p class="block__header yellow">Development</p>
          <p class="block__item">Vue.js</p>
          <p class="block__item">Vuetify</p>
          <p class="block__item">Tailwind.css</p>
          <p class="block__item">React.js</p>
          <p class="block__item">Jest</p>
          <p class="block__item">Node.js</p>
          <p class="block__item">npm, yarn</p>
        </div>
        <div class="block">
          <p class="block__header">Management and Tools</p>
          <p class="block__item">Jira</p>
          <p class="block__item">Notion</p>
          <p class="block__item">Webpack</p>
          <p class="block__item">GitHub, GitLab</p>
        </div>
        <div class="block">
          <p class="block__header blue">UI/UX Design</p>
          <p class="block__item">Figma</p>
          <p class="block__item">Sketch</p>
          <p class="block__item">Adobe Photoshop</p>
          <p class="block__item">Adobe Illustrator</p>
          <p class="block__item">Adobe After Effects</p>
        </div>
      </div>
    </div>
    <div class="works">
      <p class="experience__header">Experience</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Experience',
};
</script>
<style scoped>
.experience {
  width: 100%;
  box-sizing: border-box;
  display: grid;
  grid-template-columns: repeat(7, 1fr);
  grid-template-rows: repeat(7, 1fr);
  grid-gap: 1rem;
}

.technologies {
  grid-column: 1 / 8;
  grid-row: 3;
  display: grid;
  grid-template-columns: repeat(8, 1fr);
  grid-template-rows: 1fr;
}

.technologies__blocks {
  grid-column: 4 / 8;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: 1fr;
  grid-gap: 1rem;
  font-family: 'Spartan', sans-serif;
}

.block {
  margin-top: .5rem;
}

.block__header {
  font-size: 1rem;
  font-weight: 600;
  margin-bottom: 1rem;
}

.block__item {
  font-size: .875rem;
  line-height: 1.5rem;
}

.works {
  grid-column: 1 / 8;
  grid-row: 6;
  display: grid;
  grid-template-columns: repeat(6, 1fr);
}

.experience__header {
  font-family: 'Syne', sans-serif;
  font-size: 6vh;
  grid-column: 1 / 4;
  line-height: 1;
}

.yellow {
  color: #FFBD00;
}

.blue {
  color: #2C6FF3;
}

</style>
