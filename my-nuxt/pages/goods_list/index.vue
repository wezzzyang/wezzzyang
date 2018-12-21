<template>
  <div>
    <h2>商品列表</h2>
    <ul>
      <li :Key="item.name" v-for="item of list">
        <nuxt-link :to="'/detail/'+ item.id">{{item.name}}</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>

export default {
    data: () => {
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