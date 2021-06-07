<script context="module">
	export const prerender = true;
</script>

<script>
	import Counter from '$lib/Counter/index.svelte';
</script>

<svelte:head>
	<title>Log In</title>
</svelte:head>

<section>
	<h1>
		<div id="logo">
			<picture>
				<img src="TaxiLogo.jpg" alt="Taxi" width="200"/>
			</picture>
		</div>

		GoTaxi
	</h1>

	<h2 class="subtitle">LOG IN</h2>

	

<form action="/action_page.php" target="_self">
	<label for="email">Email:</label>
	<input type="text" id="email"><br>

	<label for="password">Password:</label>
	<input type="password" id="password"><br>

	
	<input type="submit" value="Log in">
</form>
<a href="./register">You don't have an account yet ? Register here</a>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}
	h1 {
		width: 100%;
	}
	#logo {
		position: relative;
		height: 0;
		padding: 0 0 5% 0;
		margin-left: 20%;
	}
</style>