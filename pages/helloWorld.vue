<template>
  <div class="container">
    <div>
      <h1 class="title">
        Hello World
      </h1>
      <div class="links">
        <buttonComponent />
        <p>{{ dateTime }}</p>
      </div>
    </div>
  </div>
</template>

<script>
import buttonComponent from '~/components/button.vue'
export default {
  name: 'HelloWorld',
  components: {
    buttonComponent
  },
  data () {
    return {
      dateTime: this.$moment()
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.links {
  padding-top: 15px;
}
</style>
