<script setup lang="ts">
	import LeftSide from './LeftSide.vue'
	import RightSide from './RightSide.vue'
	import Footer from './Footer.vue'


</script>

<template>
	<div class="layer">
		<LeftSide />
		<slot />
		<RightSide />
		<Footer />
	</div>
</template>

<style scoped>
	.layer {
		position: relative;
		width: 100%;
		height: 100%;
		background-color: #FAF6F1;
		/* background-color: #373737; */
		padding: 0px 10%;
		display: flex;
		flex-direction: column;
	}
</style>
