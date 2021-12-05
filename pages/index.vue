<template>
  <div>
    Hello
    <MyComponent />
    <span class="foo">Foo</span>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import MyComponent from '~/components/MyComponent.vue'

export default Vue.extend({
  components: { MyComponent },
  methods: {
    foo () {
      const foo = "bar";
    }
  }
})
</script>
