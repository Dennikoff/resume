<template>
	<div id="main-banner" class="flex"> 
		<div class="mx-auto title-container">
			<h1 class="main-title orange-gradient">Front-end</h1>
			<h2 class="main-subtitle">Developer</h2>
		</div>
		
		
	</div>
</template>

<script setup lang="ts">


</script>

<style scoped lang="scss">
.main-title {
	text-align: center;
	text-transform: uppercase;
	font-size: 12rem;
	font-weight: 900;
	line-height: 1;
	margin-inline: auto;
}

.title-container {
	position: relative;
	display: flex;
}

.main-subtitle {
	position: absolute;
	top: 100%;
	left: -5%;
	text-align: center;
	text-transform: uppercase;
	font-size: 10rem;
	line-height: 1;
	font-weight: 900;
	background: conic-gradient(from 255deg at 50% 60%, $gradien-start, $gradien-end);
  -webkit-background-clip: text;
  -webkit-text-stroke: 10px transparent;
  color: $dark;

  // -webkit-text-stroke-color: conic-gradient(from 255deg at 50% 60%, $gradien-start, $gradien-end);
}

.orange-gradient {
  background-image: conic-gradient(from 255deg at 50% 60%, $gradien-start, $gradien-end);
  color: transparent;
  background-clip: text;
  -webkit-background-clip: text;
	// animation: color-change 5s linear infinite;
}

@keyframes color-change {
    0% {
			transform: rotate(0deg);
    }

    50% {
			transform: rotate(180deg);
    }

    100% {
			transform: rotate(360deg);
    }
}

</style>