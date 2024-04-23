<script>
/* import { info } from 'sass'; */
import PageHeader from './components/PageHeader.vue';
import PageFooter from './components/PageFooter.vue';
import AppHero from './components/AppHero.vue';
import AppFounder from './components/AppFounder.vue';
import AppNewCourses from './components/AppNewCourses.vue';
import AppBookSales from './components/AppBookSales.vue';
import AppWhyCourses from './components/AppWhyCourses.vue';
import AppStatistics from './components/AppStatistics.vue';


export default  {
    components: {
        PageHeader,
        PageFooter,
        AppHero,
        AppFounder,
        AppNewCourses,
        AppBookSales,
        AppWhyCourses,
        AppStatistics,
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
        ],
        socials: [
          {
            social: "fa-brands fa-linkedin",
          },
          {
            social: "fa-brands fa-instagram",
          },
          {
            social: "fa-brands fa-facebook",
          },
          {
            social: "fa-brands fa-twitter",
          },
        ]
      };
    },
}
</script>

<template>
  <!--  passo al'array headerInfos  nelle props di PageHeader l'array headerLinks  -->
  <PageHeader :headerInfos="headerLinks" :headerSocials="socials"></PageHeader> 
  <main>
    <AppHero></AppHero>
    <AppFounder></AppFounder>
   <AppNewCourses></AppNewCourses>
   <AppBookSales></AppBookSales>
   <AppWhyCourses></AppWhyCourses>
   <AppStatistics></AppStatistics>
  </main>
  <PageFooter></PageFooter>
</template>

<style lang="scss">
@use './style/generic';
</style>
