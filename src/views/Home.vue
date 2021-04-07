<template>
  <div class="home">
    <Banner/>
    <Exchange />
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from '@/components/Banner'
import Exchange from '@/components/Exchange'

export default {
  name: 'Home',
  data: () => ({
    animate: false
  }),
  components: {
    Banner,
    Exchange
  }
}
</script>

<style>

</style>
