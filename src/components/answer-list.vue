<template>
  <section v-if="answers">
    
    <answer-list-element v-bind:key="answer" v-for="answer of answers">
      
    </answer-list-element>

  </section>
</template>

<script>
import AnswerListElement from "./answer-list-element.vue"

export default {
  name: 'AnswerList',
  props: {
    answers: Array
  },
  components: {
    AnswerListElement
  }
}
</script>

<style>

</style>