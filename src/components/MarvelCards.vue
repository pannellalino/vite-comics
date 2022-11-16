<script>
export default {
  name: 'MarvelCards',
  props:{
    cardImage: String,
    cardTitle: String
  }
}
</script>


<template>
  <div class="card">
    <img :src="cardImage" alt="">
    <h4>{{cardTitle}}</h4>
  </div>
</template>


<style lang="scss" scoped>
.card{
  padding: 10px;
  width: calc(100% / 6);
  height: 100%;
  img{
    width: 100%;
    aspect-ratio: 1/1;
    object-fit: cover;
    object-position: top;
  }
  h4{
    margin-top: 10px;
    color: white;
    font-size: .8rem;
    text-transform: uppercase;
  }
}

</style>