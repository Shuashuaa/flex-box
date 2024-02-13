<template>
	<div style="display: flex; justify-content: center; height: 100vh; padding-top: 10vh;">
		<div style="width: 70%;">
			<h1>Flex Box</h1>
			<div style="display: flex; flex-wrap: wrap; justify-content: center;">
				<div v-for="(stack1, i) in otherStacks" :key="i" style="background-color: white; display: flex; flex-grow: 4; align-items: center; justify-content: space-between; width: 200px; padding: 0 10px 0 10px; border: 1px solid rgba(52, 58, 64, 0.62); border-radius: 1px;"
				>
					<img :src="stack1.image" style="height: 30px;"/>
					
					<p style="text-decoration: underline dotted black;">{{stack1.name}}</p>
				</div>
			</div>
			<p>see more ...</p>
		</div>
	</div>
	
</template>

<script setup>
import { ref } from 'vue';

	const otherStacks = ref([
		{ name: 'HTML', image: 'https://cdn-icons-png.flaticon.com/512/174/174854.png' },
		{ name: 'CSS', image: 'https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/800px-CSS3_logo.svg.png' },
		{ name: 'JAVASCRIPT', image: 'https://static.vecteezy.com/system/resources/previews/027/127/463/original/javascript-logo-javascript-icon-transparent-free-png.png' },
		{ name: 'PHP', image: 'https://pngimg.com/d/php_PNG27.png' },
		{ name: 'MYSQL', image: 'https://upload.wikimedia.org/wikipedia/commons/7/7b/MySQL_Dolphin.jpg' },
		{ name: 'NODEJS', image: 'https://cdn-icons-png.flaticon.com/512/5968/5968322.png' },
		{ name: 'BOOTSTRAP', image: 'https://upload.wikimedia.org/wikipedia/commons/thumb/b/b2/Bootstrap_logo.svg/1280px-Bootstrap_logo.svg.png' },
		{ name: 'FIGMA', image: 'https://w7.pngwing.com/pngs/431/965/png-transparent-figma-designer-computer-icons-material-design-design-rectangle-poster-logo.png' },
		{ name: 'GIT', image: 'https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png' },
		{ name: 'GITHUB', image: 'https://cdn-icons-png.flaticon.com/512/25/25231.png' },
		{ name: 'GITLAB', image: 'https://cdn.icon-icons.com/icons2/2415/PNG/512/gitlab_original_logo_icon_146503.png' },
		{ name: 'POSTMAN', image: 'https://cdn.worldvectorlogo.com/logos/postman.svg' },
		{ name: 'BABEL', image: 'https://user-images.githubusercontent.com/3025322/87547253-bf050400-c6a2-11ea-950a-280311bc6cc8.png' },
		{ name: 'JQUERY', image: 'https://cdn.worldvectorlogo.com/logos/jquery-4.svg' },
		{ name: 'VSCODE', image: 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Visual_Studio_Code_1.35_icon.svg/2048px-Visual_Studio_Code_1.35_icon.svg.png' },
		{ name: 'NPMJS', image: 'https://static-00.iconduck.com/assets.00/npm-icon-512x512-qtfdrf37.png' },
		{ name: 'YARNPKG', image: 'https://avatars.githubusercontent.com/u/22247014?s=280&v=4' },
		{ name: 'SWEETALERT2', image: 'https://sgo.pm.ce.gov.br/_lib/libraries/grp/sweetalert/sweetalert2-9.7.2/assets/swal2-logo-square.png' }
	])
</script>

<style>
	body {
		padding: 0;
		margin: 0;
	}

	#app{
		font-family: "Roboto Mono", monospace;
	}
	@import url('https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@500&display=swap');
</style>