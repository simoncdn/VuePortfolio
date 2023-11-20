<template>
	<div class="right-side">

		<div class="cube-container">
			<span class="cube"></span>
			<span class="cube"></span>
			<span class="cube"></span>
			<span class="cube"></span>
		</div>

		<span class="line"></span>

		<p>Home</p>

	</div>
</template>

<style scoped>
	.right-side{
		position: fixed;
		top: 0;
		right: 0;
		width: 5%;
		height: calc(100vh - 50px);
		display: flex;
		flex-direction: column;
		justify-content: end;
		align-items: center;
		gap: 20px
	}
	
	.right-side p{
		writing-mode: vertical-rl;
		transform: rotate(180deg);
		color: #373737;
		font-weight: 200;
		font-size: 16px;
	}
	.line{
		width: 1px;
		height: 20%;
		background-color: #373737;
	}
	
	.cube-container{
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 20px;
	}
	.cube:first-child{
		background-color: orange;
	}
	.cube{
		width: 6px;
		height: 6px;
		background-color: #cbcbcb;
	}
</style>
