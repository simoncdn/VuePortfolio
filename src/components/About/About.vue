<script setup lang="ts">

	import Badge from "../reusable/Badge.vue";

	const languagesList = ["JavaScript", "TypeScript", "React.js", "Next.js"]
	const librariesList = ["Tailwind", "Styled-Component", "Zustand", "React-Query", "Jest", "React Testing Library", "Git", "Figma", "Nvim"]
</script>

<template>
	<div id="about" class="about">
		<div class="about-left-part">
			<div class="image-container">
				<img src="../../assets/image-profil.svg" alt="">
			</div>
		</div>

		<div class="about-right-part">
			<div class="title">
			<h2>About</h2>
			<span class="title-underline"></span>
			</div>

			<div class="about-content">

				<div class="about-subtitle">
					<h4>France</h4>
					<h4>96'</h4>
				</div>

				<div class="description-container">
					<p>Frontend developer based in France specialized in React.js and TypeScript.</p>
					<p>Passionate about crafting modern and responsive user interfaces, I bring technical expertise and a creative approach to each project. </p>
					<p>With  years of experience, I collaborate with businesses and startups to turn their ideas into high-performing, user-friendly web applications.</p>
				</div>

				<div class="hard-skills-container">

					<div class="hard-skills-top">
						<h3 class="">Languages & Frameworks</h3>

						<ul class="languages-list">
							<li v-for="language in languagesList">
								<Badge :label="language" />
							</li>
						</ul>
					</div>

					<div class="hard-skills-bottom">
					<h3 class="">Libraries & Tools</h3>
					<ul class="languages-list">
						<li v-for="library in librariesList">
							<Badge :label="library" />	
						</li>
					</ul>
					</div>

				</div>
			</div>

		</div>
	</div>
</template>

<style scoped>	
.about {
	background-color: #373737;
	/* background-color: red; */
	width: 100%;
	height: 100vh;
	display: flex;
	justify-content: space-between;
	padding: 200px 0px;
	gap: 200px;
}
.about-left-part{
	width: 50%;
	height: 100vh;
	display: flex; 
	justify-content: center;
}
.image-container{
	position: relative;
	margin-top: 100px;
	width: 600px;
	height: fit-content;
}
.image-container img{
	width: 100%;
	object-fit: cover;
	mix-blend-mode: lighten;
}

.about-right-part{
	width: 50%;
	height: 100vh;
	color: #Faf6f1;
	flex-direction: column;
	display: flex;
}
				
.title{
	position: relative;
	width: fit-content;
	padding: 0px 20px;
	display: flex;
	justify-content: center;
}
h2{
	position: relative;
	color: white;
	width: 100%;
	z-index: 10;
	font-size: 128px;
	font-weight: 600;
}
.title-underline{
	position: absolute;
	bottom: 20px;
	right: 0;
	left: 0;
	width: 100%;
	height: 50px;
	background-color: #FFA500;
}
.about-subtitle{
	display: flex;
	flex-direction: column;
	justify-content: space-between;
	gap: 10px;
	margin: 32px 0px;
}
h4{
	color: #FaF6f1;
	font-size: 20px;
	font-weight: 600;
}

.description-container{
	width: 100%;
	max-width: 600px;
	margin-bottom: 64px;
}
.description-container p{
	color: #Faf6f1;
	font-size: 16px;
	font-weight: 200;
}

.hard-skills-container{
	display: flex;
	flex-direction: column;
	gap: 50px;
}
.languages-list{
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	gap: 16px;
	margin-top: 20px;
	max-width: 360px;
}
.languages-list li{
	list-style: none;
	white-space: nowrap;
} 
</style>
