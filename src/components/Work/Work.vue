<script setup lang="ts">
	const toggle = () => {
		const work3 = document.querySelector('.work-3')
		work3.classList.toggle('active')
	}

</script>


<template>
	<div id="work" class="work">
		<h2>Work</h2>

		<button @click="toggle">Toggle</button>
		<div class="works-container">
			<div class="work-1">work-1</div>
			<div class="work-2">work-2</div>
			<div class="work-3">work-3</div>
		</div>
	</div>
</template>

<style>
.work {
	background-color: blue;
	width: 100%;
	height: 100vh;
	display: flex;
	flex-direction: column;
	gap: 20px
}
button{
 width: fit-content;
}
.works-container{
	background-color: pink;
	width: 100%;
	position: relative;
	overflow: hidden;
}
.work-1{
	background-color: white;
	width: 100%;
	height: 100vh;
}
.work-2{
	position: absolute;
	right: 0;
	top: 0;
	left: 0;
	background-color: purple;
	width: 100%;
	height: 100vh;
	transform: translateX(100%);
}
.work-3{
	position: absolute;
	right: 0;
	top: 0;
	left: 0;
	background-color: orange;
	width: 100%;
	height: 100vh;
	transform: translateX(200%);
}
.active{
	transform: translateX(0%);
}
</style>
