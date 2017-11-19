<template>
  <section>
    
    <p>question list element</p>
    {{question.title}}
    <answer-list :answers="question.answers"></answer-list>
  </section>
</template>

<script>
import AnswerList from "./answer-list.vue"


// :title="title" :answers="answers"
export default {
  name: 'QuestionListElement',
  props: {
    question: Object
  },
  components: {
    AnswerList
  }
}
</script>

<style>

</style>