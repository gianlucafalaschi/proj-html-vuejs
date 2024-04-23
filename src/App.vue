<script>
/* import { info } from 'sass'; */
import PageHeader from './components/PageHeader.vue';
import PageFooter from './components/PageFooter.vue';
import AppHero from './components/AppHero.vue';
import AppFounder from './components/AppFounder.vue';
import AppNewCourses from './components/AppNewCourses.vue';


export default  {
    components: {
        PageHeader,
        PageFooter,
        AppHero,
        AppFounder,
        AppNewCourses,
    },
    data() {
      return {
        headerLinks: [
          {
            text: 'Courses',
          },
          {
            text: 'Course Formats',
          }, 
          {
            text: 'Add Course',
          },
          {
            text: 'Pages',
          }, 
          {
            text: 'Demos',
          }, 
        ]
      };
    },
}
</script>

<template>
  <!--  passo al'array headerInfos  nelle props di PageHeader l'array headerLinks  -->
  <PageHeader :headerInfos="headerLinks"></PageHeader> 
  <main>
    <AppHero></AppHero>
    <AppFounder></AppFounder>
   <AppNewCourses></AppNewCourses>
  </main>
  <PageFooter></PageFooter>
</template>

<style lang="scss">
@use './style/generic';
</style>
