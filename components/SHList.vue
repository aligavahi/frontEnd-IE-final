<template>
<div>
  {{ref}}
  <ul v-for="item in lists" @click = "toggle(item.list)">
  {{item.list}}
  <li v-for="name in item.subl" :style="'display: ' + displays[item.list] " class="hide">
  {{name}}    
  </li>
  </ul>  
</div>
</template>

<script >
export default {
  props:{
   lists: {type: Array }
  },
  methods: {
    toggle(name){
      for (var i in this.lists) {
         if(this.lists[i].list == name)
          this.displays[this.lists[i].list] = this.displays[this.lists[i].list] == "block" ? "none":"block";
        else
          this.displays[this.lists[i].list] = "none";
      }
      this.ref="ref";
      this.ref="";
    }
  },
   data() {
    return {
      displays :{},
      ref : ""
    }
  }
}
</script>



<style scoped>
div{
  margin: 5px;
  width: 100%;
  text-align: right;
  height: 200px;
  overflow: scroll;
}
.hide{
  display: none;
}
</style>