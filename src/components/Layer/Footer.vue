<script setup lang="ts">

	const linksList = [
		{
			name: 'LinkedIn',
			link: 'https://www.linkedin.com/in/simoncdna/'
		},
		{
			name: 'Github',
			link: 'https://github.com/simoncdn'
		},
		{
			name: 'Email',
			link: 'mailto:cdna.simon@gmail.com'
		}
	]

</script>

<template>
	<div class="footer">
		<ul class="links-container">
			<li v-for="link in linksList">
				<a :href="link.link">{{link.name}}</a>
			</li>
		</ul>
	</div>
</template>


<style scoped>
	.footer {
		position: fixed;
		bottom: 0;
		right: 0;
		left: 0;
		width: calc(100% - 10%);
		margin: auto;
		height: 50px;
		display: flex;
		justify-content: left;
		align-items: center;
	}
	.links-container{
		display: flex;
		justify-content: left;
		align-items: center;
		gap: 20px;
	}
	li{
		list-style-type: none;
	}
	a{
		text-decoration: none;
		color: #373737;
		font-size: 16px;
		font-weight: 200;
	}
	a:hover{
		text-decoration: underline;
		cursor: pointer;
	}
</style>

