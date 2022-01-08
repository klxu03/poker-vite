<script setup>
	defineProps({
		card: String,
	});
</script>

<template>
	<div
		class="card_back"
		:class="{ card_1: card == '1', card_2: card == '2' }"
	></div>
</template>

<style lang="scss" scoped>
	$black: #4b4b4b;
	$dark: #707070;
	$white: #f5f5f5;
	$red: #ff5900;

	.card_back {
		position: absolute;
		width: 78px;
		height: 95px;

		background: $red;
		border: 5px solid $white;
		box-sizing: border-box;
		border-radius: 10px;
	}

	.card_1 {
		transform: rotate(-10deg);
	}

	.card_2 {
		margin-left: 45px;
		transform: rotate(10deg);
	}
</style>
