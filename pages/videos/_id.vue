<template>
  <div>
      <nuxt-child :video="video"></nuxt-child>
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
  },
  computed: {
    video() {
      return this.videos.find(v => v.id == this.$route.params.id)
    }
  }
}
</script>

<style>

</style>