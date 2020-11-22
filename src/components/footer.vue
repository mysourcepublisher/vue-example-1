<template>
  <div id="foot">
      <div id="pages">
          <a href="#">Contact Us</a>
          <a href="#">About Us</a>
          <a href="#">Privacy and Policy</a>
          <a href="#">Terms and Conditions</a>
      </div>
  </div>
</template>

<script>
export default {
    name:'Footer'
}
</script>

<style>
    #foot{
        font-family: Arial, Helvetica, sans-serif;
        margin-top: 5px;
        border-top: 2px solid rgba(0,0,0,0.5);
        padding-top: 20px;
        text-align: center;
    }
    #pages a{
        text-decoration: none;
        border: 1px solid #4d0643;
        color: #4d0643;
        padding: 10px;
        margin: 5px;
    }
    #pages a:hover{
        color: #ffffff;
        background-color: #4d0643;
    }
</style>