<script>
	let count = 0;

	$: {
		if (count > 10) {
			console.log('I am the winner!');
		}
	} //this is a reactive statement
</script>

<div class="text-white">
	<div>I am a task manager page - {count}</div>
	<button
		on:click={() => {
			count++;
			//console.log("Clicking!");
		}}
	>
		Increment
	</button>
</div>
