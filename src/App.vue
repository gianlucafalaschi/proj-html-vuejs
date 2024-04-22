<script>
/* import { info } from 'sass'; */
import PageHeader from './components/PageHeader.vue';
import PageFooter from './components/PageFooter.vue';
import StartRevolution from './components/StartRevolution.vue';


export default  {
    components: {
        PageHeader,
        PageFooter,
        StartRevolution,
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
    <StartRevolution></StartRevolution>
  </main>
  <PageFooter></PageFooter>
</template>

<style lang="scss">
@use './style/generic';
</style>
