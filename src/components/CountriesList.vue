<template lang="html">
    <div>
      <label for="country_select">Select a Country:</label>
      <select id="country_select" v-model="selectedCountry">
      <option disabled value=""> Select a country </option>
      <option v-for="(country) in countries" :value="country"> {{country.name}} </option>
    </select>
    </div>
</template>

<script>
import ListItem from './ListItem.vue';


export default {
  name: 'countries-list',
  props: ['countries'],
  components: {
    "list-item": ListItem
  }
}
</script>

<style lang="css" scoped>
</style>
