<template>
  <div>
    <h1>{{ title }}</h1>
    <p>{{ desc }}</p>

    <div>
      <nuxt-link to="/notice">文章详情</nuxt-link>
    </div>
    <div>
      <nuxt-link :to="{name:'member',params:{id:999}}">会员中心</nuxt-link>
    </div>
    <div>
      <nuxt-link :to="{name:'other',query:{id:666}}">其他页面</nuxt-link>
    </div>

  </div>
</template>

<script>

export default {
  data(){
    return {
      title: '首页',
      desc: 'this is my nuxt demo.'
    }
  }
}
</script>

<style>

</style>

