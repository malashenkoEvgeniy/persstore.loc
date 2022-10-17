<template>
  <div class="home">
    Hello wold
  </div>
</template>

<script>

export default {
  mounted () {
    this.getPoint()
  },
  methods: {
    getPoint () {
      this.axios.get('http://localhost/api')
        .then(res => {
          console.log(res)
        })
    }
  }
}
</script>
