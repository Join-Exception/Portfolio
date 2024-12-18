<script>
	export let y;
	let tabs = [
		{ name: 'Projects', link: '#projects' },
		{ name: 'About Me', link: '#about' }
	];
</script>

<header
	class={'sticky top-0 z-[10] flex items-center justify-between px-5 duration-150' +
		(y > 0
			? ' border-none bg-gray-900 bg-opacity-20 py-3 backdrop-blur-md'
			: ' border-transparent bg-transparent py-6')}
>
<title>JoinException's Portfolio</title>
	<div class="flex w-full items-center justify-between">
		<!-- Left: Name -->
		<a href="/" class="flex-shrink-0 sm:ml-10">
			<h1>
				<b
					class="font-montserrat text-2xl font-bold text-white duration-200 hover:inline-block hover:bg-gradient-to-r hover:from-emerald-500 hover:to-purple-500 hover:bg-clip-text hover:text-transparent"
				>
				JoinException
				</b>
			</h1>
		</a>

		<!-- Center: Tabs -->
		<div class="hidden items-center gap-6 text-center text-xl sm:flex">
			{#each tabs as tab}
				<a href={tab.link} class="font-montserrat text-white duration-200 hover:text-gray-300">
					<p>{tab.name}</p>
				</a>
			{/each}
		</div>

		<!-- Right: Button -->
		<div class="flex-shrink-0">
			
		</div>
	</div>
</header>
