<script>
	import Recipe from './Recipe.svelte'
	import { goto } from '@roxi/routify'
	import Break from '../../components/Break.svelte'
</script>

<div class="body">

	<div class="header">
		<p class="headerTitle">Vo-edsel</p>
		<div class="menu">
			<button class="button" on:click={() => $goto('../signin')}>
				<p>Sign in</p>
			</button>
			<button class="button" on:click={() => $goto('../signup')}>
				<p>Sign up</p>
			</button>
		</div>
	</div>
	
	<div class="main">
		<p class="title">Recepten van de dag</p>
		<Break/>
		<Recipe
			header="VOMBER"
			body="Goed lichaam"
		/>
	</div>

</div>

<style>
	.body {
		box-sizing: border-box;
		display: flex;
		margin: 0px;
		flex-direction: column;
		background-color: #f8f8f8;
	}

	.body > * {
		flex: 1 100%;
	}

	.header {
		background-color: #56a75680 ;
	}

	p.headerTitle {
		color: #f8f8f8;
		font-size: 4em;
		font-weight: 300;
		text-align: center;
		font-family: Cambria;
	}

	.menu {
		display: flex;
		flex-direction: row;
		justify-content: flex-end;
	}

	.button {
		margin: 5px;
		background-color: #56a75680;
		padding: 5px;
		border-radius: 5px;
	}

	.main {
		background-color: #f8f8f8;
		display: flex;
		align-items: center;
		flex-direction: column;
	}

	p.title {
		font-size: 2em;
		font-weight: 300;
		text-align: center;
		font-family: Cambria;
		margin: 5px;
	}

	p {
		margin: 0px;
	}
	
</style>