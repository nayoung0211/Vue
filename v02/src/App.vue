<script>
export default{
  data() {
    return{
      score: 60,
      subscribe : 2677,
    }
  },
};
</script>

<template>
<h1 v-if="score >= 90">평점 A</h1>
<h1 v-else-if="score >= 80">평점 B</h1>
<h1 v-else-if="score >= 70">평점 C</h1>
<h1 v-show="score != 60">이 영역은 v-show에서 처리하고 있습니다.</h1>
<h1 v-show="score == 60">이 60 영역은 v-show에서 처리하고 있습니다.</h1>
<h2>구독자 수 : {{ subscribe }}</h2>
<p>{{ `오늘의 행운 숫자 : `+Math.ceil(Math.random()*45) }}</p>
<h1 v-text="channel"></h1>
<h2 v-text="subscribe"></h2>
</template>

<style></style>
