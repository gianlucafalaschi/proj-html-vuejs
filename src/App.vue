<script>
/* import { info } from 'sass'; */
import PageHeader from './components/PageHeader.vue';
import PageFooter from './components/PageFooter.vue';
import AppHero from './components/AppHero.vue';


export default  {
    components: {
        PageHeader,
        PageFooter,
        AppHero,
    },
    data() {
      return {
        headerLinks: [
          {
            text: 'Courses',
          },
         /*  {
            text: 'Course Formats',
          }, */
        ]
      };
    },
}
</script>

<template>
  <PageHeader></PageHeader>
  <main>
    <AppHero></AppHero>
  </main>
  <PageFooter></PageFooter>
</template>

<style lang="scss">
@use './style/generic';
</style>
