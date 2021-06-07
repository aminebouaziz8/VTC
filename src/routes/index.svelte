<script context="module">
	export const prerender = true;
</script>

<script>
	import Counter from '$lib/Counter/index.svelte';
</script>

<svelte:head>
	<title>Home</title>
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

	<h2 class="subtitle">Always on time</h2>

	<h2>
		Whether you’re visiting Paris and want to book a taxi from the train station <strong>to 
		your hotel</strong>, need to get a cab from the city <strong>back home</strong> or are flying out from Paris 
		airports and need an <strong>airport express taxi service</strong> in Paris to get you there as 
		quickly as possible, you can rely on us.
	</h2>

	<p>Order your next ride !</p>

<form>
	<label for="pickup">Pickup:</label>
	<input type="text"><br>

	<label for="destination">Destination:</label>
	<input type="text"><br>

	<label for="date">Date:</label>
	<input type="date" id="date" name="ridedate" value="2021-31-05" min="today" max="2021-12-31"><br>

	<label for="nbpassengers">Number of passengers:</label>
	<select id="nbpassengers" name="nbpassengers">
		<option value= "">Choose an option</option>
		<option value="1">1 passenger</option>
		<option value="2">2 passengers</option>
		<option value="3">3 passengers</option>
		<option value="4">4 passengers</option>
		<option value="5">5 passengers</option>
		<option value="6">6 passengers</option>
	</select><br>

	<input type="submit" value="Book">
</form>
<a href="./login">LOG IN</a>
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
