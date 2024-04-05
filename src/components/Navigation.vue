<template>
	<nav id="navigation">

			<div class="flex justify-content-center">
				<div class="navigation-container mt-5 py-3 px-5">
					<div class="flex gap-5" >
						<div v-for="navigationItem in navigationList" :key="navigationItem.title">
							<a :href="navigationItem.link">
								{{ navigationItem.title }}
							</a>
						</div>
					</div>
				</div>
			</div>

	</nav>
</template>

<script setup lang="ts">

const navigationList = [
	{
		title: 'Главная',
		link: '#'
	},
	{
		title: 'Обо мне',
		link: '#'
	},
	{
		title: 'Опыт',
		link: '#'
	},
	{
		title: 'Портфолио',
		link: '#'
	},
	{
		title: 'Контакты',
		link: '#'
	},

]

</script>

<style scoped lang="scss">
#navigation {
	position: fixed;
	z-index: 10;
	top: 0;
	left: 0; 
	right: 0;
	
}

.navigation-container {
	border: 1px solid $main-color;
	border-radius: 30px;
	background-color: $dark;
	font-weight: 700;
}


</style>