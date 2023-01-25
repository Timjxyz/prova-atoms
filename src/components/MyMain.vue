<template>
<main>
  <MyArticlesSection/>
  <!-- <MyArticlesSectionSm/> -->
</main>
</template>

<script>
import MyArticlesSection from './partials/MyArticlesSection.vue';
// import MyArticlesSectionSm from './partials/MyArticlesSectionSm.vue';
export default {
  name: 'MyMain',
  components: {
    MyArticlesSection,
    // MyArticlesSectionSm,
  },
  data(){
    return{
      
    }
  }
  
}
</script>


<style scoped lang="scss">
 .container::after{
    display: table;
    content: "";
    clear: both;
}
</style>
