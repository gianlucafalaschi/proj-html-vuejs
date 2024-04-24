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
            text: 'Blog'
          },
          {
            text: 'Courses'
          },
          {
            text: 'Home'
          },
          {
            text: 'Membership A..'
          },
          {
            text: 'Shortcodes'
          },
          {
            text: 'Typography'
          },
        ],
        footerBlog: [
          {
            image: 'photo-1517520287167-4bbf64a00d66-75x75',
            title: 'Our main target is to "Developing Yourself as a Leader"',
            date: 'August 9, 2018',
          },
          {
            image: 'photo-1490376840453-5f616fbebe5b-75x75',
            title:'Those Other College Expenses You Arent \'t Thinking About',
            date: 'June 3, 2015',
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
  <!-- passo all'array footerLinksInfos nelle props di PageFooter
  l'array footerLinks -->
  <PageFooter :footerLinksInfos="footerLinks" :blogInfos="footerBlog"></PageFooter>
</template>

<style lang="scss">
@use './style/generic';
</style>
