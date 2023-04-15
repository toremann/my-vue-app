<template>
    <div>
      <p v-if="loading">Loading...</p>
      <p v-else>{{ data }}</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        data: null,
        loading: true
      }
    },
    async created() {
      const response = await fetch(process.env.VUE_APP_API, {
        headers: {
          "X-API-KEY": process.env.VUE_APP_X_API_KEY
        }
      })
      const data = await response.json()
      this.data = data
      this.loading = false
    }
  }
  </script>
  