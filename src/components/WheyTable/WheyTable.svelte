<!-- WheyTable.svelte -->

<script>
	import WheyData from '$lib/WheyData.json';
</script>

<table class="w-full text-sm text-left text-emerald-500 dark:text-white">
	<thead class="text-xs text-emerald-700 uppercase bg-emerald-50 dark:bg-emerald-700 dark:text-white">
		<tr>
			<th scope="col" class="px-6 py-3">Product</th>
			<th scope="col" class="px-6 py-3">Merk</th>
			<th scope="col" class="px-6 py-3">Omschrijving</th>
			<th scope="col" class="px-6 py-3">100gr eiwit</th>
			<th scope="col" class="px-6 py-3">Gr eiwit per 100gr product</th>
			<th scope="col" class="px-6 py-3">Verpakking</th>
			<th scope="col" class="px-6 py-3">Prijs</th>
			<th scope="col" class="px-6 py-3">Winkel</th>
			<th scope="col" class="px-6 py-3">Meer info</th>
		</tr>
	</thead>
	<tbody>
		{#each WheyData as whey}
			<tr class="bg-white border-b dark:bg-emerald-800 dark:border-emerald-700">
				<th class="px-6 py-2">{whey.Product}</th>
				<td class="px-6 py-2">{whey.merk}</td>
				<td class="px-6 py-2">{whey.Omschrijving}</td>
				<td class="px-6 py-2">{whey["100gr eiwit"]}</td>
				<td class="px-6 py-2">{whey["Gr eiwit per 100gr product"]}</td>
				<td class="px-6 py-2">{whey.Verpakking}</td>
				<td class="px-6 py-2">{whey.Prijs}</td>
				<td class="px-6 py-2">{whey.Winkel}</td>
				<td class="px-6 py-2"><a href={whey["Meer info"]}>Meer info</a></td>
			</tr>
		{/each}
	</tbody>
</table>
