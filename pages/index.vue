<template>
  <Tutorial />
</template>

<script lang="ts">
import Vue from 'vue'
import { Person } from '../interfaces/Person'

export default Vue.extend({
  data () {
    return {
      people: [] as Person[]
    }
  },
  computed: {
    peopleWithPhone() : Person[] {
      return this.people.filter(p => p.mobile)
    }
  }
})
</script>
