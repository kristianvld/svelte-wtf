<script>
	let tall = [1, 2, 3];

	$: sum = tall.reduce((a, b) => a + b);

	$: {
		console.log('ny sum:', sum);
	}

	let nytt = 4;
</script>

<h1>Tall:</h1>
{tall.join(', ')} = {sum}

<br />
<br />
<h3>Legg til: {nytt}</h3>
<input type="number" bind:value={nytt} />
<button on:click={(e) => (tall = [...tall, nytt])}>Legg til</button>
