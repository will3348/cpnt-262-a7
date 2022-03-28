<template>
  <div  class="body">
    <TheCard v-for="card in cards" :key="card.id"
  :card="card">
    </TheCard>
  </div>
</template>
<script>
import TheCard from './cards/TheCard.vue'
const cards = [
  {
    title: "Badminton" , 
    text:"Badminton is a racquet sport played using racquets to hit a shuttlecock across a net. " ,
    tags:["rachet","2people","sport"],
    image:require('../assets/images/badminton.webp'),
    id:1
  },

  {
    title: "Pingpong" , 
    text:"Table tennis, is a sport in which two or four players hit a lightweight ball, back and forth across a table using small solid rackets." ,
    tags:["rachet","2people","sport"],
    image:require('../assets/images/pingpong.jpg'),
    id:2

  },

  {
    title: "Dodgeball" , 
    text:"Dodgeball is a team sport in which players on two teams try to throw balls and hit opponents, while avoiding being hit themselves." ,
    image:require('../assets/images/dodgeball.jpg'),
    id:3

  },


]
export default {
  components: {
    TheCard
  },
  data(){
    return {cards}
  }
}

</script>
<style scoped>
.body {
  display:flex;
  justify-content: center;
  gap: 30px;
}
</style>

