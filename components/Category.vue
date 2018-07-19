<template>
  <div id= "cont" :style="'background-image: '+src">
  <div id = "title">
  {{title}}
  </div>
</div>
</template>

<script >

export default {
  props:["src","title"]
}
</script>



<style scoped>
#cont{
  padding: 5%;
  margin: 3px;
  background-color: #888888;
  width: 100%;
  position:relative;
}

#title{
  position:absolute;left:50%;bottom:0;
  transform:translate(-50%,0%);
  -ms-transform:translate(-50%,0%);
  background-color: rgba(100,100,100,.5);
  width: 100%;
  text-align: center;
}

</style>