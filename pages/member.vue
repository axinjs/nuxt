<template>
  <div>
    <h1>{{ title }}</h1>
    <p>会员编号-{{ $route.params.id }}</p>
    <p>{{ desc }}</p>



    <nuxt-link to="/">返回首页</nuxt-link>

  </div>
</template>

<script>

export default {
  data(){
    return {
      title: '会员中心',
      desc: 'this is my member page.'
    }
  },
  
}
</script>

<style>

</style>

