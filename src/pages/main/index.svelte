<script>
	import Recipe from './Recipe.svelte'
	import { url } from '@roxi/routify'
</script>

<body>
	<div class="header">
		<h1>VOMB</h1>
	</div>
	<div class="main">
		<div>
			<a href={$url('./vomb')}>VoorbeeldLink</a>
			<Recipe
				header={"Snack: Madison Beer"}
				body={"Een kanker boeiend verhaal over madison beer... Grapje ze is gewoon lekker"}
				src={"https://i.dailymail.co.uk/1s/2020/12/15/01/36848506-0-image-a-77_1607996735722.jpg"}
			/>
		</div>
		<div>
			<Recipe
				header={"Titel van recept"}
				body={"Body text body text body text body text body text"}
				src={"https://hips.hearstapps.com/hmg-prod.s3.amazonaws.com/images/cardi-b-reebok-1605107359.jpg"}
			/>
		</div>
		<div>
			<Recipe
				header={"Snack: Ariana Grande"}
				body={"Ariana is hier niet de echte snack. ZIj lijkt op Cardi B. De echte snack is Darion natuurlijk"}
				src={"https://hips.hearstapps.com/hmg-prod.s3.amazonaws.com/images/screen-shot-2020-11-17-at-12-58-32-pm-1605639574.png"}
			/>
		</div>
	</div>
</body>

<style>
	body {
		box-sizing: border-box;
	}

	.header {
		background-color: #D0585890 ;
		padding: 30px;
		text-align: center;
		color: antiquewhite;
	}

	.main {
		display: flex;
		align-items: center;
		flex-direction: column;
	}

	h1 {
		color: #F7F7F7;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
</style>