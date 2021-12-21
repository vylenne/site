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
      <div class="works__blocks">
        <div class="work">
          <p class="work__title">Uscreen.tv / Middle Frontend dev / Sep 2021 – present</p>
          <p class="work__description">Created referral program for stores in uscreen.tv. Fixed
            critical and non-critical bugs, supported the code. Studied 4 books about typography and
            interfaces, turned knowledge into action.</p>
        </div>
        <div class="work">
          <p class="work__title">Amberdata / Vue.js frontend developer / Sep 2019 - Sep 2020</p>
          <p class="work__description">Design and development of projects related to data collection
            and visualization. Took part in the renovation of the project, which was written on
            Backbone and is now written entirely on Vue.js with using Vuetify.js.</p>
        </div>
        <div class="work">
          <p class="work__title">MediaTarget / Frontend dev / Jul 2018 – Nov 2018</p>
          <p class="work__description">Adaptation of the rvpn portal for the mobile version
            (https://rusvpn.com). Developed some pages with adaptation with receiving
            content(articles, news) from a backend on a Cryptoportal. Full cycle of creation from
            scratches to real pages with stylus styles and page blocks according to all customer
            constraints (with animations and prepared scripts for interaction with backend)</p>
        </div>
      </div>
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
  height: 100vh;
  overflow-y: scroll;
}

.experience__header {
  font-family: 'Syne', sans-serif;
  font-size: 5vh;
  grid-column: 1 / 4;
  line-height: 1;
}

.technologies {
  display: grid;
  grid-template-columns: repeat(8, 1fr);
  grid-template-rows: 1fr;
  margin-top: 5rem;
}

.works {
  display: grid;
  grid-template-columns: repeat(8, 1fr);
  grid-template-rows: 1fr;
  margin-top: 4rem;
}

.technologies__blocks {
  grid-column: 4 / 8;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: 1fr;
  grid-gap: 1rem;
  font-family: 'Spartan', sans-serif;
}

.works__blocks {
  grid-column: 4 / 8;
  font-family: 'Spartan', sans-serif;
  overflow-y: scroll;
}

.block {
  margin: .5rem 0;
}

.work {
  margin-bottom: 2rem;
}

.block__header,
.work__title {
  font-size: 1rem;
  font-weight: 600;
  margin-bottom: .5rem;
}

.block__item,
.work__description {
  font-size: .875rem;
  line-height: 1.5rem;
}

.yellow {
  color: #FFBD00;
}

.blue {
  color: #2C6FF3;
}

</style>
