<script context="module">
	const userDB = {
		kristian: {
			navn: "Kristian in't Veld",
			studie: 'KomTek',
		},
	};

	export async function preload({ params }) {
		const bruker = userDB[params.user];

		if (bruker) {
			return { bruker };
		} else {
			this.error(404, `User <code>${params.user}</code> not found`);
		}
	}
</script>

<script>
	export let bruker;
</script>

<h1>Bruker:</h1>
<p>Navn: {bruker.navn}</p>
<p>Studie: {bruker.studie}</p>
