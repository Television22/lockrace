<script>
	export let week = 0;
	export let status = ' ';
</script>

<div class="font-bold bg-white rounded-sm m-1 shadow-md p-2 grid grid-cols-5">
	<div>Week: {week}</div>
	{#if status == 'W'}
		<div>✔️</div>
	{/if}
	{#if status == 'L'}
		<div>❌</div>
	{/if}
	{#if status == 'T'}
		<div>➖</div>
	{/if}
	{#if status == ' '}
		<div />
	{/if}
</div>
