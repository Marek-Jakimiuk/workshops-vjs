<template>
  <section>
    <p>question list</p>

    <question-list-element v-bind:key="question" v-for="question in questions" :question="question">
    </question-list-element>
  </section>
</template>

<script>
import QuestionListElement from "./question-list-element.vue"

export default {
  name: 'QuestionList',
  props: {
    questions: Array
  },  
  components: {
    QuestionListElement
  }
}
</script>

<style>

</style>