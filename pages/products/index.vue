<template>
	<div class="flex">
		<div id="left">
			<div >
				<h5>{{group_name}}</h5>
				<div class="flex">
					<div class="flex">
						<button> صفحه قبل</button>
						<div> صفحه {{cur_page}} از {{total_page}} </div>
						<button> صفحه بعد</button>
					</div> 
					<div style="margin-left: 50%;"> 
						<select>
							<option>محبوبیت</option>
							<option>قیمت</option>
							<option>تخفیف</option>
						</select>
						مرتب سازی
					</div>
				</div>
			</div>
			<div id="results">
				<Product v-for = "product in products"
				 :b_name = "product.bname"
				 :p_name = "product.pname"
				 :src = "product.src"
				 :price = "product.price"
				 :real_price = "product.real_price"
				 />
			</div>
		</div>
		<div id="right">
			<SHContainer type = "list" title = "دسته بندی ها"/>
			<SHContainer type = "select-brand" title = "بر اساس برند"/>
			<SHContainer type = "select-color" title = "رنگ"/>
		</div>
	</div>
</template>

<script>
import SHContainer from '@/components/SHContainer'
import Product from '@/components/Product'
export default {
  components: {
  	SHContainer,
  	Product
  },
  data(){
  	return{
  		group_name:"موبایل",
  		total_page:5,
  		cur_page:2,
  		products : [ {id:1,bname:"apple",pname:"تلفن",src:"",price:100,real_price:50},
  					 {id:2,bname:"nokia",pname:"تلفن",src:"",price:300,real_price:50},
  					 {id:3,bname:"samsung",pname:"یخچال",src:"",price:100,real_price:50},
  					 {id:4,bname:"asus",pname:"تلویزیون",src:"",price:500,real_price:100},
  					 {id:5,bname:"samsung",pname:"ماشین لباس شویی",src:"",price:100,real_price:50},
  					 {id:6,bname:"nokia",pname:"کمد",src:"",price:100,real_price:50},
  					 {id:7,bname:"samsung",pname:"لباس",src:"",price:605,real_price:600},
  					 {id:8,bname:"nokia",pname:"میز",src:"",price:100,real_price:50},
  					 {id:9,bname:"apple",pname:"موبایل",src:"",price:100,real_price:50},
  					 {id:10,bname:"apple",pname:"موبایل",src:"",price:100,real_price:50},
  					 {id:11,bname:"asus",pname:"تلفن",src:"",price:125,real_price:50},
  					 {id:12,bname:"asus",pname:"یخچال",src:"",price:100,real_price:50},
  					 {id:13,bname:"htc",pname:"کمد",src:"",price:250,real_price:230},
  					 {id:14,bname:"htc",pname:"لباس",src:"",price:120,real_price:100}
  		]
  	}
  }
}
</script>

<style scoped>
#left{
	width: 100%;
	padding: 2%;
}
h5{
	text-align: right;
	clear: both;
}
#right{
	width: 20%;
}
.flex{
	display: flex;
}

button{
	margin-left: 5px;
	margin-right: 5px;
	border: 1px solid black;
}

#results{
display: table;
width: 100%;
margin-top: 30px;
}
</style>
