<script lang="ts">
import { defineComponent } from 'vue';
import NavLinks from '../components/NavLinks.vue';
import HeroBox from '../components/HeroBox.vue';
import UmbrellaShow from '../components/UmbrellaShow.vue'
import DolapoDev from '../components/DolapoDev.vue';
import ImagineCreate from '../components/ImagineCreate.vue';
import StatementView from '../components/statements/StatementView.vue'
import CreativeDev from '../components/creativedev/CreativeDev.vue'
import ProjectsView from '../components/ProjectsView.vue'
import ScrollView from '../components/ScrollView.vue'

export default defineComponent({
  components: {
    NavLinks,
    HeroBox,
    UmbrellaShow,
    DolapoDev,
    ImagineCreate,
    StatementView,
    CreativeDev,
    ProjectsView,
    ScrollView
  },
  methods: {

  },
});
</script>

<template>
  <main class="min-h-[100vh]">
    <NavLinks />
    <HeroBox />
    <UmbrellaShow />
    <DolapoDev />
    <ImagineCreate />
    <StatementView />
    <CreativeDev />
    <ProjectsView />
    <ScrollView />
  </main>
</template>

<style scoped>
main {
  background-color: #ECEBE9;
}
</style>
