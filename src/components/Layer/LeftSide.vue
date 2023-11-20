<template>
	<div class="left-side">
		<span class="line"></span>
		<p>Portfolio 2023</p>
		<span class="line"></span>
	</div>
</template>


<style scoped>
.left-side {
	position: fixed;
	top: 0;
	left: 0;
	width: 5%;
	height: 100vh;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	gap: 20px;
}

.left-side p {
	writing-mode: vertical-rl;
	transform: rotate(180deg);
	color: #373737;
	font-weight: 200;
	font-size: 16px;
}

.line {
	width: 1px;
	height: 35%;
	background-color: #373737;
}
</style>
