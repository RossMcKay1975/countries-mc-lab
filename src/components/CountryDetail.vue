<template lang="html">
  <article v-if="country">
    <p>{{ country.name }}</p>
    <p>{{ country.region }}</p>

  </article>
</template>

<script>
export default {
  name: 'country-detail',
  props: ['country']
}
</script>

<style lang="css" scoped>
</style>
