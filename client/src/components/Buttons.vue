<script setup></script>

<template>
	<div class="buttons">
		<a>
			<div class="button">
				<h1>Raise</h1>
			</div>
		</a>

		<a>
			<div class="button">
				<h1>Check</h1>
			</div>
		</a>

		<a @click="console.log('hello')">
			<div class="button">
				<h1>Fold</h1>
			</div>
		</a>
	</div>
</template>

<style lang="scss" scoped>
	$black: #4b4b4b;
	$dark: #707070;
	$light: #cccccc;
	$white: #f5f5f5;
	$red: #ff5900;
	$green: #00971d;

	.buttons {
		// position: absolute;
		// top: 80%;
		// left: 65%;
		margin-top: 49px;
		margin-left: 10%;

		width: 500px;
		display: flex;
		flex-direction: horizontal;
		justify-content: space-around;
	}

	.button {
		width: 120px;
		height: 90px;
		border: 5px solid #00971d;
		border-radius: 20px;
	}

	h1 {
		font-family: Rubik;
		font-style: normal;
		font-weight: 600;
		font-size: 32px;
		line-height: 38px;
		/* identical to box height */

		color: #00971d;
	}
</style>
