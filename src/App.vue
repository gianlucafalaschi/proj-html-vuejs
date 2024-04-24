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
import AppReviews from './components/AppReviews.vue';


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
        AppReviews,
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
        ],
        footerLinks: [
          {
            title: 'PAGES',
            text: 'Blog'
          },
          {
            title: 'PAGES',
            text: 'Courses'
          },
          {
            title: 'PAGES',
            text: 'Home'
          },
          {
            title: 'PAGES',
            text: 'Membership A..'
          },
          {
            title: 'PAGES',
            text: 'Shortcodes'
          },
          {
            title: 'PAGES',
            text: 'Typography'
          },
        ],

        
      };
    },
}
</script>

<template>
  <!--  passo al'array headerInfos  nelle props di PageHeader l'array headerLinks e l'array socials  -->
  <PageHeader :headerInfos="headerLinks" :headerSocials="socials"></PageHeader> 
  <main>
    <AppHero></AppHero>
    <AppFounder></AppFounder>
   <AppNewCourses></AppNewCourses>
   <AppBookSales></AppBookSales>
   <AppWhyCourses></AppWhyCourses>
   <AppStatistics></AppStatistics>
   <AppReviews></AppReviews>
  </main>
  <!-- passo all'array aboutLinks nelle props di PageFooter
  l'array footerLinks -->
  <PageFooter :aboutLinks="footerLinks"></PageFooter>
</template>

<style lang="scss">
@use './style/generic';
</style>
