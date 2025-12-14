<script lang="ts">
	import { page } from "$app/state";
</script>

<main class="min-h-screen bg-white flex items-center justify-center p-6">
	<div class="text-center">
		<h1 class="text-6xl font-bold text-gray-900 mb-4">Error {page.status}</h1>
		<p class="text-lg text-gray-600 mb-8">{page.error?.message ?? "Something went wrong."}</p>
		<a href="/" class="bg-black text-white px-6 py-3 text-sm font-medium rounded-sm hover:bg-gray-800 transition-colors inline-block">
			Go back home
		</a>
	</div>
</main>
