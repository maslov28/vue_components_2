<template>
  <base-card 
    v-for="item in array" 
    :key="item.id"
    :title="item.title"
  >
  </base-card>
</template>

<script>
import BaseCard from './BaseCard.vue'
export default {
  components: { BaseCard },
  props: ['array']
}
</script>