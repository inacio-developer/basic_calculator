<script setup>
const emit = defineEmits(['updateOperator'])

const onSelect = (event) => {
  emit('updateOperator', event.target.value)
}
</script>

<template>
  <select class='select' @change="onSelect">
    <option value="Addition">Addition (+)</option>
    <option value="Subtraction">Subtraction (-)</option>
    <option value="Multiplication">Multiplication (*)</option>
    <option value="Division">Division (/)</option>
  </select>
</template>

<style>
.select {
  display: block;
  width: 305px;
  outline: none;
  border: 1.9px solid #224573;
  border-radius: 3px;
  padding: 10px 8px;
  margin-bottom: 5px;
  font-size: 16px;
}
</style>