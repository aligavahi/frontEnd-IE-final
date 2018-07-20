<template>
<div id="cont">
 <form action="" method="">
   <input class="align-right" type="text" name="search-brand" placeholder="جست و جوی برند">
   <div v-for = "item in items" class="inputs">{{item}}<input type="checkbox" :name="item" value=true></div>
 </form>
</div>
</template>

<script >
export default {
  props:{
   lists: {type: Array }
  },
  methods: {
    getBrands(){
      
      this.ref="ref";
      this.ref="";
    }
  },
   data() {
    return {
      items :["apple","htc","asus","samsung"],
      ref : ""
    }
  }
}
</script>



<style scoped>
#cont{
  margin: 5px;
  width: 100%;
  height: 200px;
  overflow: scroll;
}

input{
  margin: 5px;
  float: right;
}

.inputs{
  margin: 2px;
  border-bottom: 1px solid black;
}

.align-right{
  text-align: right;
  width: 100%;
}
</style>