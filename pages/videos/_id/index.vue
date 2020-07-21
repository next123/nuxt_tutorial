<template>
  <div>
      <h2>page {{ video.name}}</h2>
      <nuxt-link :to="`/videos/${video.id}/edit`">
        <button>edit</button>
      </nuxt-link>
  </div>
</template>

<script>
export default {
props: ['video']
}
</script>

<style>

</style>