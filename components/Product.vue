<template>
<span id= "P_cont" :style="'font-size: ' + size + ';background-color: ' + color" @mouseover="emph()" @mouseout="norm()">
  <nuxt-link to="/detail">
        <div class="image" :style="'background-image: url('+src+')'"> </div>
        <div>  {{b_name}} </div>
        <div class="gray">  {{p_name}} </div>
        <div> <span class="red"> {{real_price}} </span> <span class="dec"> {{price}} </span> </div>
        <div class="red"> تومان </div>
  </nuxt-link>
  <div class="percentage"><span class="middle">{{off_percent}}</span></div>
</span>
</template>

<script >

export default {
  props:["src","b_name","p_name","price","real_price"],
  methods: {
      norm(){
        this.size = ".75em";
        this.color = "rgba(100,100,100,.5)";
      },

      emph(){
        this.size = ".8em";
        this.color = "rgba(200,200,200,.5)";
      }
  },
   data() {
    return {
      size:".7em",
      color:"rgba(100,100,100,.5)",
      off_percent:"10%"
    }
  }
}
</script>



<style scoped>

#P_cont {
  box-sizing: border-box;
  padding: 3px;
  margin: 10px;
  background-color: #888888;
  background-repeat: no-repeat;
  background-size: 100%;
  background-position: center;
  width: 20%;
  height: 250px;
  position:relative;
  display: inline-flex;
  flex-flow: column;
  text-align: center;
}
.gray {
  color: gray;
}

.red {
  color: red;
}

.dec{
  text-decoration: line-through;
}

.image{
  width: 100%;
  height: 150px;
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
}

.percentage{
  position: absolute;
  right: -15px;
  top: -15px;
  border-radius: 50%;
  width: 50px;
  height: 50px;
  background-color: pink;
  text-align: center;
  display: table;
}

.middle{
display: table-cell;
vertical-align: middle;
}
</style>