<template>
  <ul>
    <li v-for="food in foods"><a @click="$goRoute(food.route)">{{food.context}}</a>
    </li>
  </ul>
</template>

<script>
  export default {
    name: '',
    data () {
      return {
        foods: [
          {
            context: '红烧猪蹄',
            route: '/'
          },
          {
            context: '清蒸鹿茸',
            route: '/'
          },
          {
            context: '薯条',
            route: '/'
          },
          {
            context: '汉堡',
            route: '/'
          }
        ]
      }
    }
  }
</script>

<style scoped>

</style>
