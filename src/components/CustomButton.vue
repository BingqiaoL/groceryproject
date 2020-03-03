<template>
    <div>
    <button v-on:click="increment">+</button>
    <button v-on:click="decrement">-</button>
    <br><br>
    <div id="div_cnt">
        {{counter}} </div>
    </div>
</template>
         

<script>
export default {
  
  data(){
    return{
        counter:0
    }
  },

  methods:{
      increment:function(){ 
          if(this.counter < 10) {
            this.counter++;
          } else {
              alert("You can not buy more than 10 items!");
          }
          
      }, 
      decrement:function(){
          if(this.counter > 0) {
              return this.counter--;
          } else {
              return this.counter;
          }
      }
    } 
          
}
</script>

<style scoped> 
button{
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    text-align: center; 
    color: #bb0d38a8; }
</style>
               