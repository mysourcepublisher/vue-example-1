<template>
  <div id="app">
    <Header title="Store" value="20"/>
    <div class="ingr">
      <div class="ingredients" v-for="(ingredients,index) in ingredients" :key="'ing'+index">
        <SalesItem :title="ingredients.title" :image="ingredients.picture" :price="ingredients.price"/>
      </div>
    </div>
    <Footer/>
  </div>
</template>

<script>
  import Header from './components/header'
  import Footer from './components/footer'
  import SalesItem from './components/SalesItem'
  export default {
    data:()=>{
      return {
        ingredients:[
          {title:"Toy Car",picture:"toy_car.jpg",price:200.05},
          {title:"Bunny",picture:"bunny.jpg",price:120.00},
          {title:"Dachshund",picture:"dachshund.jpg",price:500.00},
          {title:"Toy Car",picture:"toy_car.jpg",price:200.00},
          {title:"Bunny",picture:"bunny.jpg",price:120.00},
          {title:"Dachshund",picture:"dachshund.jpg",price:500.00}
        ]
      }
    },
    name:'App',
    components:{
      Header,
      Footer,
      SalesItem
    }
  }
</script>

<style>
.ingredients{
  display: inline-block;
}
</style>
