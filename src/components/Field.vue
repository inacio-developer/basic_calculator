<script setup>
import { toRefs } from 'vue'

const props = defineProps({
  value: Number,
  setValue: Function
})

const onInput = (event) => {
  props.setValue(event.target.value)
}
</script>

<template>
  <input type="number" class="number" :value="value" @input="onInput" />
</template>

<style scoped>
.number {
  display: block;
  width: 300px;
  outline: none;
  border: 1.9px solid #224573;
  border-radius: 3px;
  padding: 10px 2px;
  text-align: center;
  margin-bottom: 5px;
  font-size: 16px;
}
</style>