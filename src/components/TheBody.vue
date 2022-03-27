<template>
  <div class="body">
    <TheCards v-for="card in cards" :key="card.id">
      <div name="title">
          {{card.image}}
      </div>
      
    </TheCards>
  </div>
</template>
<script>
import TheCards from './cards/TheCards.vue'

export default {
  components: {
    TheCards
  },
}
</script>
