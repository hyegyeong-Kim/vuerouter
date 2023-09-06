<template>
  <div v-for="(a,i) in 블로그" :key="i">
    <h5 @click="$router.push('/detail/' + i)">{{a.title}}</h5>
    <p>{{a.date}}</p>
  </div>
  
</template>

<script>
export default {
    name : 'List',
    props : {
      블로그 : Array
    }
}
</script>

<style>

</style>