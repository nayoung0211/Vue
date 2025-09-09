<script setup>
import { reactive,ref } from 'vue';

const count = ref(0);

const obj1 = reactive({
  name : "kimg",age : 33
})

</script>
<template>
<p>count : {{ count }}</p>
<p>obj1 : {{ obj1.name }}/{{ obj1.age }}</p>
</template>