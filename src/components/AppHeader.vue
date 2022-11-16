<script>
  export default {
    name: 'AppHeader',
    data(){
      return{
        menu:[
          {
            text: 'Characters',
            href: '#',
            current: false
          },
          {
            text: 'Comics',
            href: '#',
            current: true
          },
          {
            text: 'Movies',
            href: '#',
            current: false
          },
          {
            text: 'TV',
            href: '#',
            current: false
          },
          {
            text: 'Games',
            href: '#',
            current: false
          },
          {
            text: 'Collectibles',
            href: '#',
            current: false
          },
          {
            text: 'Videos',
            href: '#',
            current: false
          },
          {
            text: 'Fans',
            href: '#',
            current: false
          },
          {
            text: 'News',
            href: '#',
            current: false
          },
          {
            text: 'Shop',
            href: '#',
            current: false
          }
        ]
      }
    }
  }
</script>


<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="/dc-logo.png" alt="Logo">
      </div>
      <nav>
        <ul>
          <li v-for="(link, index) in menu" :key="index">
            <a :class="{active : link.current}" :href="link.href">{{link.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>


<style lang="scss" scoped>
header{
  width: 100%;
  height: 120px;
  background-color: white;
  .container{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    vertical-align: middle;
    nav{
      height: 100%;
      ul{
        display: flex;
        height: 100%;
        li{
          height: 100%;
          list-style: none;
          padding: 0 10px;
          a{
            display: flex;
            align-items: center;
            height: 100%;
            text-decoration: none;
            color: black;
            text-transform: uppercase;
            &:hover{
              color: #0D69F6;
              border-bottom: 5px solid #0D69F6;
            }
          }
        }
      }
    }
  }
}
img{
  height: 80px;
}
</style>