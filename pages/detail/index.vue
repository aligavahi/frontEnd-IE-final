<template>
<div>
	<TabTable :product_id="1"/>
	<CommonProducts/>
</div>
</template>

<script>

import CommonProducts from '@/components/CommonProducts'
import TabTable from '@/components/TabTable'
export default {

  components: {
  	CommonProducts,
  	TabTable
  },
  data(){
  	return{
  	products : [ {id:1,bname:"apple",pname:"تلفن",src:"/products/m1.jpeg",price:100,real_price:50},
  					 {id:2,bname:"nokia",pname:"تلفن",src:"/products/m2.jpeg",price:300,real_price:50},
  					 {id:3,bname:"samsung",pname:"یخچال",src:"/products/m1.jpeg",price:100,real_price:50},
  					 {id:4,bname:"asus",pname:"تلویزیون",src:"/products/m3.jpeg",price:500,real_price:100},
  					 {id:5,bname:"samsung",pname:"ماشین لباس شویی",src:"/products/m1.jpeg",price:100,real_price:50},
  					 {id:6,bname:"nokia",pname:"کمد",src:"/products/m1.jpeg",price:100,real_price:50},
  					 {id:7,bname:"samsung",pname:"لباس",src:"/products/m3.jpeg",price:605,real_price:600},
  					 {id:8,bname:"nokia",pname:"میز",src:"/products/m1.jpeg",price:100,real_price:50},
  					 {id:9,bname:"apple",pname:"موبایل",src:"/products/m1.jpeg",price:100,real_price:50},
  					 {id:10,bname:"apple",pname:"موبایل",src:"/products/m2.jpeg",price:100,real_price:50},
  					 {id:11,bname:"asus",pname:"تلفن",src:"/products/m1.jpeg",price:125,real_price:50},
  					 {id:12,bname:"asus",pname:"یخچال",src:"/products/m2.jpeg",price:100,real_price:50},
  					 {id:13,bname:"htc",pname:"کمد",src:"/products/m1.jpeg",price:250,real_price:230},
  					 {id:14,bname:"htc",pname:"لباس",src:"/products/m3.jpeg",price:120,real_price:100}
  		]
  	}
  }
}
</script>

<style scoped>

</style>
