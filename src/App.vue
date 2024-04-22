<script>
import PageHeader from './components/PageHeader.vue';
import PageFooter from './components/PageFooter.vue';

export default  {
    components: {
        PageHeader,
        PageFooter,
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

  </main>
  <PageFooter></PageFooter>
</template>

<style lang="scss">
@use './style/generic';
</style>
