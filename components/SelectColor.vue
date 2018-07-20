<template>
<div id="cont">
<button v-for = "item in items" type="submit" :style="'background-color:'+item" :name="item" @click="submit_data(item)"/>
</div>
</template>

<script >
export default {
  props:{
   lists: {type: Array }
  },
  methods: {
    submit_data(name){

    }
  },
   data() {
    return {
      items :["blue","red","black","white","purple","green","yellow","brown","gray","khaki","orange","pink"],
    }
  }
}
</script>



<style scoped>
#cont{
  margin: 5px;
  width: 100%;
  height: 200px;
  display: table;
}

button{
  margin: 10px;
  width: 30px;
  height: 30px;
}
</style>