<template>
  <main>
    <MainJumbotron />
    <MainAbout />
    <MainSubscribe />
    <MainSpeakers />
    <MainProgram />
    <MainMap />
    <MainLocation />
    <MainNews />
    <MainTickets />
    <MainPresentation />
    <MainSponsor />
  </main>
</template>

<script>

import MainJumbotron from './MainJumbotron.vue';
import MainAbout from './MainAbout.vue';
import MainSubscribe from './MainSubscribe.vue';
import MainSpeakers from './MainSpeakers.vue';
import MainProgram from './MainProgram.vue';
import MainMap from './MainMap.vue';
import MainLocation from './MainLocation.vue';
import MainNews from './MainNews.vue';
import MainTickets from './MainTickets.vue';
import MainPresentation from './MainPresentation.vue';
import MainSponsor from './MainSponsor.vue';

export default {
  name: 'MainContent',
  components: {
    MainJumbotron,
    MainAbout,
    MainSubscribe,
    MainSpeakers,
    MainProgram,
    MainMap,
    MainLocation,
    MainNews,
    MainTickets,
    MainPresentation,
    MainSponsor
  }
}
</script>

<style scoped lang="scss">

</style>
