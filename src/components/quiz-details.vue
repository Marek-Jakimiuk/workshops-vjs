<template>
  <section v-if="quiz">
    <h2> {{ quiz.name }}</h2>
    <p>{{ quiz.categoryName}}</p>
    <div>

      <img :src="quiz.promo"/>
    </div>
  </section>

</template>

<script>
export default {
  name: 'QuizDetails',
  props: {
    quiz: Object
  }
}
</script>

<style>

</style>
