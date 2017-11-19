<template>
  <section v-if="quiz">
    <h2> {{ quiz.name }}</h2>
    <p>{{ quiz.categoryName}}</p>
    <div>

      <img :src="quiz.promo"/>
    </div>


    <question-list :questions="quiz.questions"></question-list>
  </section>

</template>

<script>
import QuestionList from "./question-list.vue"

export default {
  name: 'QuizDetails',
  props: {
    quiz: Object
  },
  components: {
    QuestionList
  },
}
</script>

<style>

</style>
