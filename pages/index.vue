<template>
<content>
	<ImageSlider style="width: 90%" class="main_row"/>
	<div  class="main_row" >
	<Category title="بچگانه"/>
	<Category title="زنانه"/>
	<Category title="مردانه"/>	
	</div>	
	<div  class="main_row" style="text-align: center;" >
		<b style="width: 100%;">
		بهترین ها را از ما خرید کنید
		</b>
	</div>
	<div  class="main_row">
		<Khabarnameh style = "margin-right: 30px"/>
		<Spon/>
	</div>
</content>
</template>

<script>

import ImageSlider from '@/components/ImageSlider'
import Category from '@/components/Category'
import Spon from '@/components/Spon'
import Khabarnameh from '@/components/Khabarnameh'

export default {
  components: {
    ImageSlider,
    Category,
    Spon,
    Khabarnameh
  }
}
</script>

<style scoped>
.main_row{ 
  margin: 1% 5% 1% 5%;
  display: flex;
}
</style>