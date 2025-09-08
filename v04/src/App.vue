<script>
import ChildComponents from './components/LocalChild.vue';
export default{
  components : {
    ChildComponents
  },
  methods : {
    callFunction(var1){
      console.log('자식 컴포넌트에서 보낸 이벤트를 수신했어요.'+var1)
    }
  }
}
</script>

<template>
<h1>나는 부모 컴포넌트</h1>
<ChildComponents @create-post="callFunction"/>
</template>

<style>
</style>
