<script setup>
	import DeckCard from "@/components/DeckCard.vue";
</script>

<template>
	<div class="container">
		<div class="cards">
			<DeckCard />
			<DeckCard />
			<DeckCard />
			<DeckCard />
			<DeckCard />
		</div>
		<div class="pot">
			<div class="current">
				<h2>40</h2>
			</div>
			<div class="total">
				<p>total 6000</p>
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

	.container {
		width: 800px;
		height: 400px;
		margin: 45px auto 0;

		border-radius: 50%;
		background: $green;
		display: flex;
		flex-direction: column;
		justify-content: center;
	}

	.pot {
		position: absolute;
		width: 290px;
		height: 70px;

		margin-left: 270px;
		margin-top: 280px;
	}

	.pot .current {
		width: 256px;
		height: 61px;
		background: $white;
		border-radius: 17px;

		display: flex;
		flex-direction: horizontal;
		justify-content: center;
	}

	.current h2 {
		width: 41px;
		height: 38px;

		font-family: Rubik;
		font-style: normal;
		font-weight: normal;
		font-size: 32px;
		text-align: center;

		color: $black;
	}

	.pot .total {
		position: absolute;
		width: 127px;
		height: 40px;
		margin-top: -77px;
		margin-left: 170px;

		/* Light Gray */

		background: $light;
		border-radius: 25px;

		display: flex;
		flex-direction: horizontal;
		justify-content: center;
	}

	.total p {
		font-family: Rubik;
		font-style: normal;
		font-weight: normal;
		font-size: 16px;

		color: $black;
		text-align: center;
	}

	.cards {
		margin: auto;
		width: 700px;
		display: flex;
		flex-direction: row;
		justify-content: space-around;
	}
</style>
