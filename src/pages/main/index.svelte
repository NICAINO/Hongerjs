<script>
	import Recipe from './Recipe.svelte'
</script>

<main>
	<div class="header">
		<h1>VOMB</h1>
	</div>
	<body>
		<div>
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
	</body>
</main>

<style>
	.header {
		background-color: #6dff79c4 ;
		padding: 30px;
		text-align: center;
		color: antiquewhite;
	}
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}
	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
	@media (min-width: 640px) {
		main {
			max-width: 600px;
		}
	}
</style>