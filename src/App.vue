<script setup>
import Title from './components/Title.vue'
import Field from './components/Field.vue'
import Select from './components/SelectOperator.vue'
import Result from './components/Result.vue'
import { reactive, computed } from 'vue'

const state = reactive({
  numbA: 0,
  numbB: 0,
  operator: '+',
})

const result = computed(() => {
  switch (state.operator) {
    case '+':
      return state.numbA + state.numbB
    case '-':
      return state.numbA - state.numbB
    case '/':
      return state.numbB !== 0 ? state.numbA / state.numbB : 'Error'
    case '*':
      return state.numbA * state.numbB
    default:
      return 0
  }
})

const updateNumbA = (number) => {
  state.numbA = Number(number)
}

const updateNumbB = (number) => {
  state.numbB = Number(number)
}

const updateOperator = (operator) => {
  state.operator =
    operator === 'Addition'
      ? '+'
      : operator === 'Subtraction'
      ? '-'
      : operator === 'Division'
      ? '/'
      : '*'
}
</script>

<template>
  <div class="container">
    <Title />
    <Field :value="state.numbA" :setValue="updateNumbA" />
    <Field :value="state.numbB" :setValue="updateNumbB" />
    <Select @updateOperator="updateOperator" />
    <Result :result="result" />
  </div>
</template>