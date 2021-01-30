<div class="break">
    <div class="line"/>
    <div class="diagonal"/>
    <div class="diagonal"/>
    <div class="line"/>
</div>

<style>
    .break {
		display: flex;
		justify-content: center;
		flex-direction: row;
		align-items: center;
	}

	.line {
		height: 2px;
		width: 75px;
		margin: 10px;
		background-color: #56a75680;
	}

	.diagonal {
		height: 3px;
		width: 10px;
		background-color: #56a75680;
		transform: skewY(130deg);
	}
</style>