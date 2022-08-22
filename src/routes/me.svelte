<script>
	import WeekRecord from '../components/WeekRecord.svelte';

	const mockRecord = [
		{
			week: 1,
			status: 'W'
		},
		{
			week: 2,
			status: 'L'
		},
		{
			week: 3,
			status: 'T'
		},
		{
			week: 4,
			status: 'L'
		},
		{
			week: 5,
			status: 'W'
		},
		{
			week: 6,
			status: 'W'
		},
		{
			week: 7,
			status: 'W'
		},
		{
			week: 8,
			status: 'W'
		},
		{
			week: 9,
			status: 'W'
		},
		{
			week: 10,
			status: 'W'
		},
		{
			week: 11,
			status: ' '
		},
		{
			week: 12,
			status: ' '
		},
		{
			week: 13,
			status: ' '
		},
		{
			week: 14,
			status: ' '
		},
		{
			week: 15,
			status: ' '
		},
		{
			week: 16,
			status: ' '
		}
	];
</script>

<div class="flex flex-row mt-5">
	<div class="basis-1/4" />
	<div class="basis-1/2">
		<div class="rounded-lg bg-white text-center">
			<div class="avatar placeholder p-8">
				<div class="bg-neutral-focus text-neutral-content rounded-full w-24">
					<span class="text-3xl">U</span>
				</div>
			</div>
			<h1 class="font-bold">Username</h1>
			<h2 class="font-thin">8-2</h2>
		</div>
	</div>
	<div class="basis-1/4" />
</div>

<ul class="list-none mt-5 mx-2">
	{#each mockRecord as record}
		<li>
			<WeekRecord week={record.week} status={record.status} />
		</li>
	{/each}
</ul>
