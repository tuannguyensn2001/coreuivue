<template>
  <div>
    <Main/>
  </div>
</template>

<script>
import Main from "./components/Main";
export default {
  name: 'App',
  components: {
    Main
  }
}
</script>

<style lang="scss">
  // Import Main styles for this application
  @import 'assets/scss/style';
</style>
