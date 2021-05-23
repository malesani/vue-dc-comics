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
      <div class="jumbotrom">
        <img src="../assets/img/jumbotron.jpg" alt="">
      </div>
      <div class="boton-volante">Current Series</div>
      <div class="comics">
        <ul>
          <li class="comic" v-for="(comic, index) in comics" :key="index">
            <img :src="comic.thumb" alt="">
            <span>{{comic.series}}</span>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
import comics from "../assets/data/dc-comics.js";
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
      ],
      comics
    }
  },
  mounted(){
    console.log(comics);
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
    position: relative;
   .jumbotrom{
     width: 100%;
     height: 300px;
     overflow: hidden;
     color: black;
     img{
       width: 100%;
       height:700px;
     }
    }
    .boton-volante{
      position: absolute;
      left: 18%;
      top: 40%;
      height: 35px;
      padding: 10px;
      background-color: #0282F9;
      color: white;
      text-transform: uppercase;
    }
    .comics{
      width: 100%;
      height: 400px;
      padding: 1% 10% ;
      background-color: #1C1C1C;
      overflow: auto;
      ul{
        display: flex;
        flex-wrap: wrap;
        padding-top: 15px;
        color: white;
        .comic{
          width: calc(100% / 7);
          height: 150px;
          margin: 15px 15px 70px 10px ;
          
          position: relative;
          img{
            width: 100%;
            height: 170px;
          }
        }
      }
    }
  }
</style>