<template>
  <div>
    <h1>{{ title }}</h1>
    <p>{{ desc }}</p>

    <nuxt-link to="/">返回首页</nuxt-link>

  </div>
</template>

<script>
import axios from 'axios'
export default {
  transition:'only',
  data(){
    return {
      title: '',
      desc: 'this is my notice page.'
    }
  },
  head(){
    return {
      title: this.title,
      meta: [{
        hid: "description",
        name: "description",
        content: "this is my notice page"
      },{
        hid: 'viewport',
        name: 'viewport',
        content: 'width=device-width, initial-scale=1.0'
      }]
    }
  },
  // asyncData(){
  //   return axios.get('https://www.easy-mock.com/mock/5abdd9ce7a17b12a1c9965c5/example/news')
  //   .then(data=>{
  //     console.log(data)
  //     return { title: data.data.title }
  //   })
  // },
  // async asyncData (){
  //   let { data } = await axios.get('https://www.easy-mock.com/mock/5abdd9ce7a17b12a1c9965c5/example/news')
  //   return { title: data.data.title }
  // }
}
</script>

<style>

</style>

