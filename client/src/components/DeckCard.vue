<script setup>
	import clubs from "@/assets/suits/Clubs.svg";
	import diamonds from "@/assets/suits/Diamonds.svg";
	import hearts from "@/assets/suits/Hearts.svg";
	import spades from "@/assets/suits/Spades.svg";

	defineProps({
		card: String,
	});
</script>

<template>
	<div class="card_front">
		<h1>K</h1>
		<img alt="suit" :src="diamonds" class="suit" />
	</div>
</template>

<style lang="scss" scoped>
	$black: #4b4b4b;
	$dark: #707070;
	$white: #f5f5f5;
	$red: #ff5900;

	.card_front {
		width: 120px;
		height: 150px;

		background: $white;
		border: 5px solid $dark;
		box-sizing: border-box;
		border-radius: 10px;
	}

	h1 {
		margin-top: 0;
		margin-left: 21px;
		width: 42px;
		height: 43px;

		font-family: Mitr;
		font-style: normal;
		font-weight: normal;
		font-size: 56px;

		color: $red;
	}

	.suit {
		margin-top: 0px;
		margin-left: 52px;

		width: 40px;
		height: 49px;
	}
</style>
