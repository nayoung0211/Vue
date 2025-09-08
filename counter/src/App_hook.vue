<script setup>
import{ref,computed} from 'vue';

  const cnt = ref(0);
  const oddEven = computed(() => (cnt.value%2) ? '홀수' : '짝수');
  const counter = () => cnt.value++;

</script>
<template>
  <p>{{ cnt }}</p>
  <p>홀짝 판별: {{ oddEven }}</p>
  <button @click="counter">click</button>
</template>