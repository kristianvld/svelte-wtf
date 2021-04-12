<svelte:head>
	<title>Sapper project template</title>
</svelte:head>

<h1>Hallo Verden!</h1>

<h2>Brukere:</h2>
<ul>
	<li>
		<a href="/users/kristian">kristian</a>
	</li>
</ul>

<style>
	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		text-align: center;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
	}
</style>
