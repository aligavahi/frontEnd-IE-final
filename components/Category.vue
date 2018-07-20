<template>
<div id= "cont" :style="'background-image: url('+src+')'" @mouseover="emph()" @mouseout="norm()" >
  <nuxt-link :to="{path : link}">
      <div id = "title" :style="'font-size: ' + size + ';background-color: ' + color" >
      {{title}}
      </div>
  </nuxt-link>
</div>
</template>

<script >

export default {
  props:["src","title","link"],
  methods: {
      norm(){
        this.size = "1em";
        this.color = "rgba(100,100,100,.5)";
      },

      emph(){
        this.size = "1.5em";
        this.color = "rgba(200,200,200,.5)";
      }
  },
   data() {
    return {
      size:"1em",
      color:"rgba(100,100,100,.5)"
    }
  }
}
</script>



<style scoped>

#cont {
  padding: 5%;
  margin: 3px;
  background-color: #888888;
  background-repeat: no-repeat;
  background-size: 100%;
  background-position: center;
  width: 100%;
  position:relative;
}

#title{
  position:absolute;left:50%;bottom:0;
  transform:translate(-50%,0%);
  -ms-transform:translate(-50%,0%);
  width: 100%;
  text-align: center;
  color: white;
}

</style>