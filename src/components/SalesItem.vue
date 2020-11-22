<template>
  <div id="salesitem">
      <div class="item-header">
          <h1>{{title}}</h1>
      </div>
      <img v-bind:src="require('../assets/'+image)" height="200" width="350"/>
      <div id="price">
          <p id="price">Price : {{price}}</p>
      </div>
  </div>
</template>

<script>
export default {
    name:"SalesItem",
    props:{
        title:String,
        image:String,
        price:Number
    }
}
</script>

<style>
#salesitem{
    border:1px solid black;
    margin:10px;
    padding: 0;
    width: 350px;
    border-radius: 10px;
    text-align: center;
}
.item-header{
    color: #ffffff;
    background-color: #410458;
    margin: 0;
    top: 0;
    padding:20px;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
}
</style>
