<template>
  <div>
      <h1>
          Videos:
      </h1>
      <div v-for="video in videos" :key="video.id">
        <nuxt-link :to="`/videos/${video.id}`">{{video.name}}</nuxt-link>  
        </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      videos: [
        {
          id: 1,
          name: 'Intro to Nuxtjs'
        },
         {
          id: 2,
          name: 'Intro to Nuxtjs 2'
        },
         {
          id: 3,
          name: 'Intro to Nuxtjs 3'
        }
      ]
    }
  }
}
</script>

<style>

</style>