<script setup>
	import HandCard from "@/components/HandCard.vue";

	const username = "Player 2";
	const bal = 5000;
</script>

<template>
	<div class="big-container">
		<div class="bid">
			<div class="amt">
				<p>500</p>
			</div>
		</div>

		<div>
			<HandCard card="2" />
			<HandCard card="1" />
			<div class="player">
				<!-- <Card /> -->
				<div class="text">
					<h1>{{ username }}</h1>
					<h2>{{ bal }}</h2>
				</div>
			</div>
		</div>
	</div>
</template>

<style lang="scss" scoped>
	$black: #4b4b4b;
	$dark: #707070;
	$light: #cccccc;
	$white: #f5f5f5;
	$red: #ff5900;
	$green: #00971d;

	.big-container {
		width: 568px;
		height: 100px;
		display: flex;
		flex-direction: row;
		padding-top: 49px;

		// margin: 0 42% 0 28%;
		margin-left: 10%;
	}

	.player {
		width: 270px;
		height: 100px;

		background: $dark;
		border-radius: 0.9375em;

		margin-left: 45px;

		display: flex;
		flex-direction: row;
		align-items: left;
		justify-content: left;
	}

	.text {
		margin: 0;
		display: flex;
		flex-direction: column;
		align-items: left;
		justify-content: left;
		margin-left: 120px;
	}

	h1 {
		margin-top: 18px;

		font-family: Rubik;
		font-style: normal;
		font-weight: 600;
		font-size: 28px;

		color: $white;
	}

	h2 {
		margin-top: -10px;

		font-family: Rubik;
		font-style: normal;
		font-weight: normal;
		font-size: 24px;

		color: $white;
	}

	.bid {
		// position: absolute;
		display: flex;
		flex-direction: row;
		justify-content: center;
		margin-top: auto;
		margin-right: 58px;
	}

	.bid .amt {
		width: 210px;
		height: 85px;
		background: $red;
		border-radius: 36px;
	}

	.bid p {
		font-family: Rubik;
		font-style: normal;
		font-weight: 600;
		font-size: 32px;

		color: $white;
		text-align: center;
		margin-bottom: 5px;
		padding-bottom: 5px;
	}
</style>
