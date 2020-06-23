<template>
  <div>
    <h1>{{ title }}</h1>
    {{ 'id-'+ $route.query.id }}
    <p>{{ desc }}</p>

    <nuxt-link to="/">返回首页</nuxt-link>

  </div>
</template>

<script>

export default {
  data(){
    return {
      title: '我是其他内容',
      desc: 'this is my other page.'
    }
  }
}
</script>

<style>

</style>

