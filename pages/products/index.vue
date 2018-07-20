<template>
	<div style="display: flex;">
		<div id="left">
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
export default {
  components: {
  	SHContainer
  }
}
</script>

<style>
#left{
	width: 100%;
}
#right{
	width: 20%;
}
</style>
