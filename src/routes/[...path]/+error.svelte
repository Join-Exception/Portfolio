<script>
	import { page } from '$app/stores';
</script>

<div class="flex h-screen flex-col items-center justify-center bg-white bg-opacity-5 text-center">
	<h1 class="mb-4 text-4xl font-bold text-white">Oops! Page Not Found</h1>
	<p class="text-lg text-gray-300">We couldn't find the page you're looking for.</p>
	{#if $page?.error}
		<div
			class="mt-6 w-full max-w-md rounded-lg border border-gray-600 bg-emerald-950 bg-opacity-85 p-6 shadow-lg"
		>
			{#if $page?.status}
				<p class="text-gray-400">
					<strong class="text-gray-200">Page Status:</strong>
					{$page?.status}
				</p>
			{/if}
			{#if $page?.error?.message}
				<p class="mt-2 text-gray-400">
					<strong class="text-gray-200">Error Message:</strong>
					{$page?.error?.message}
				</p>
			{/if}
		</div>
	{/if}
</div>
