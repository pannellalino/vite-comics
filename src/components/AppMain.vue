<script>

import MarvelCards from "./MarvelCards.vue";

import card from '../data/card';


  export default {
    name: 'AppMain',
    components:{
      MarvelCards
    },
    data(){
      return{
        card
      }
    }
  }
</script>


<template>
  <main>
    <div class="container">
      <MarvelCards
      v-for="(hero, index) in card"
      :key="index"
      :cardImage="hero.thumb"
      :cardTitle="hero.series"
      />
      <div class="button">
        <button><a href="#">LOAD MORE</a></button>
      </div>
    </div>
  </main>
  
</template>


<style lang="scss" scoped>
main{
  padding: 50px 0 20px 0;
  background-color: #151515;
  display: flex;
  align-items: center;
  h1{
    color: white;
  }
  .container{
    display: flex;
    flex-wrap: wrap;
    button{
      margin-top: 30px;
      background-color: #0D6EFF;
      padding: 10px 50px;
      border: 1px solid black;
      &:hover{
        background-color: transparent;
        border: 1px solid #0D6EFF;
      }
      a{
        text-decoration: none;
        color: white;
      }
    }
  }
  .button{
    width: 100%;
    display: flex;
    justify-content: center;
  }
}
</style>