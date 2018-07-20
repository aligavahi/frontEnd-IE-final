<template>
<div id= "cont" >
  <upper>
    <button @click = "toggle()">
      <img src="/shcontainer/minus.svg" :style="'display: '+ img1">
      <img src="/shcontainer/pluse.svg" :style="'display: '+ img2">
    </button>
    <h5>{{title}}</h5>
  </upper>
  <div :style="'display: '+ lower">
    <SHList v-if = "type == 'list'" :lists = "[
                    {list: 'نام دسته 1' , subl:['نام زیر دسته ۱', 'نام زیر دسته 2', 'نام زیر دسته 3']} ,
                    {list: 'نام دسته 2' , subl:['نام زیر دسته ۱']} ,
                    {list: 'نام دسته 3' , subl:['نام زیر دسته ۱', 'نام زیر دسته 2']} ,
                    {list: 'نام دسته 4' , subl:['نام زیر دسته ۱', 'نام زیر دسته 2', 'نام زیر دسته 3']} ,
                    {list: 'نام دسته 5' , subl:['نام زیر دسته ۱', 'نام زیر دسته 2', 'نام زیر دسته 3']} ,
                    {list: 'نام دسته 6' , subl:['نام زیر دسته ۱', 'نام زیر دسته 2', 'نام زیر دسته 3']} 
              ]" />
    <SearchBrand v-if = "type == 'select-brand'" />
  </div>
</div>
</template>
<script >
import SHList from '@/components/SHList'
import SearchBrand from '@/components/SearchBrand'
export default {
  props:["title","type"],
  components:{
    SHList,
    SearchBrand
  },
  methods: {
      toggle(){
        if(this.img1 == "none")
        {
          this.img1 = "block";
          this.img2 = "none";
          this.lower = "block";
        }
        else{
          this.img1 = "none";
          this.img2 = "block";
          this.lower = "none"; 
        }
      }
  },
   data() {
    return {
      img1:"block",
      img2:"none",
      lower : "block"
    }
  }
}
</script>



<style scoped>
#cont{
    background-color: rgb(200,200,200);
}
upper {
  margin: 3px;
  display: flex;
  width: 100%;
  position:relative;
}

h5{
  text-align: right;
  width: 100%;
  margin-left: 10%;
  margin-right: 2px;
}

button{
  background-color: transparent;
  width: 20%;
  margin: 2px;
}

</style>