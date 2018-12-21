<template>
  <div>
    <h2>详情页面</h2>
    {{$route.params.id}}
      <h1  v-for="item of list" v-if="item.id == $route.params.id">{{item.id}}:{{item.name}}:{{item.price}}</h1> 
  </div>
</template>

<script>

export default {
  data:() => {
   return {
     list: [
      {id: '009',name: 'iphone100', price: 20000 },
      {id: '008',name: 'huawei10000', price: 88888},
      {id: '007',name: 'chuizi1001', price: 9999}
      ]
    } 
  }
}
</script>

<style>
  
</style>