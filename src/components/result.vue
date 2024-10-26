<script setup>
const props = defineProps({
  result: [Number, String]
})
</script>

<template>
  <div class="resultShow">
    <h3 class="resultTitle">Result: </h3>
    <span class="result">{{ result }}</span>
  </div>
</template>

<style>
    .resultShow {
        width: 300px;
        height: 200px;
        border: 2px solid#224573;
    }

    .resultTitle {
        text-align: center;
        text-transform: uppercase;
        color: #224573;
    }

    .result {
        display: block;
        text-align: center;
        font-size: 20px;
    }
</style>