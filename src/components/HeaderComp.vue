<template>
  <div>
    <nav class="first-nav">
      <img src="../assets/img/dc-logo.png" alt="">
      <ul>
        <li v-for="(link,index) in links" :key="index">
          {{link.text}}
        </li>
      </ul>
    </nav>
    <nav class="second-nav">
      <h1>Content goes here</h1>
    </nav>
  </div>
</template>

<script>
export default {
  
  data(){
    return{
      links:[
        {
          text : "Characters",
          url : "/",
          current : false
        },
        {
          text : "Comics",
          url : "/",
          current : false
        },
        {
          text : "Movies",
          url : "/",
          current : false
        },
        {
          text : "TV",
          url : "/",
          current : false
        },
        {
          text : "Games",
          url : "/",
          current : false
        },
        {
          text : "Collectibles",
          url : "/",
          current : false
        },
        {
          text : "Videos",
          url : "/",
          current : false
        },
        {
          text : "Fans",
          url : "/",
          current : false
        },
        {
          text : "News",
          url : "/",
          current : false
        },
        {
          text : "Shops",
          url : "/",
          current : false
        },
      ]
    }
    
  }
}
</script>

<style lang="scss">
  .first-nav{
    
    height: 80px;
    padding: 1% 10%;
    display: flex;
    justify-content:space-between ;
    align-items: center;
    background-color: white;
    img{
      height: 60px;
    }
    ul{
      li{
        display:inline-block;
        padding-left: 20px;
        font-size: 15px;
        
      }
    }
  }
  .second-nav{
    height: 80px;
    padding: 1% 10%;
    display: flex;
    align-items: center;
    color: white;
    background-color: black;
  }
</style>