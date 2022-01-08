<script setup>
	// This starter template is using Vue 3 <script setup> SFCs
	// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
	import Player from "@/components/Player.vue";
	import Table from "@/components/Table.vue";
	import Buttons from "@/components/Buttons.vue";
</script>

<template>
	<div class="container">
		<Player style="padding-top: 25px" />
		<Table />
		<div class="player">
			<Player />
			<Buttons />
		</div>
	</div>
</template>

<style lang="scss">
	$black: #4b4b4b;
	$dark: #707070;

	.container {
		margin: auto;
		height: 720px;
	}

	#app {
		font-family: Rubik;

		// -webkit-font-smoothing: antialiased;
		// -moz-osx-font-smoothing: grayscale;

		background: $black;
		// color: #2c3e50;
		// margin: 0;
		min-height: 100%;
		min-width: 100%;
		// height: 739px; // Bull stuff how mac height is only 739px tall
	}

	.player {
		display: flex;
		flex-direction: horizontal;
	}
</style>
