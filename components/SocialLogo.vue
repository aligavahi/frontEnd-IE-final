<template>
	<div id="container">
			<a href="#">
				<img class="logo" src='/social-logo/facebook.png' onmouseover="this.src='/social-logo/facebook-red.png';" onmouseout="this.src='/social-logo/facebook.png';" />
			</a>
            <a href="#">
            	<img class="logo" src='/social-logo/twitter.png' onmouseover="this.src='/social-logo/twitter-red.png';" onmouseout="this.src='/social-logo/twitter.png';" />
			</a>
            <a href="#">
            	<img class="logo" src='/social-logo/google.png' onmouseover="this.src='/social-logo/google-red.png';" onmouseout="this.src='/social-logo/google.png';" />
            </a>
	</div>
</template>


<style scoped>
	#container{
		width: 80%;
		height: 50px;
		align-items: center;
		justify-content: center;
	}

	a{
		width: 80%;
		height: 40px;
		display: flex;
	}

	.logo{
		vertical-align: middle;
		width: 30px;
		height: 30px;
		margin: 5px;
		border-radius: 50%;
		border: 1px solid black;

	}

</style>