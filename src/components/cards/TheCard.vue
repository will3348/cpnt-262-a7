<template>
  <div class="card">
    <div class="card-image">
      <img :src="card.image"/>
    </div>
    <div class="card-title">
      {{card.title}}
    </div>
    <div class="card-text">
      {{card.text}}
    </div>
    <div v-if="card.tags" class="card-tag">
      Tags:{{card.tags.join(",")}}
    </div>
    <div class="card-CTA">
      <button>Learn More</button>
    </div>
    
  </div>
</template>
<script>
export default {name: 'TheCard',
  props: {
  card: {
      type: Object,
      required: true,
  	},
  }
}

</script>

<style scoped>
 .card{
   border: 1px solid black;
   width: 300px;
   height: 500px;
   margin-top:30px;
 }
 img{
   width: 300px;
   height: 250px;
 }
 .card-title{
   font-size: 45px;
   font-weight: bolder;
 }
 .card-text{
   margin: 15px;
 }
 button{
  margin-top :30px;
  color: aqua;
  background-color: brown;
  width: 100px;
  height: 30px;
 }
</style>