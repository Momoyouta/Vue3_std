<template>
  <div class="person">
    <h2>姓名{{name}}</h2>
    <h2>年龄{{age}}</h2>
    <button @click="changename">修改名字</button>
  </div>
</template>

<script lang="ts" setup>
  import { ref } from 'vue'
  //数据
  defineOptions({
    name:'Person'
  })
  let name = ref('张三')
  let age = ref(18)

  //方法
  function changename(){
    name.value = 'zwr'
  }
</script>

<style lang="scss" scoped>

</style>