<script>
	export let y;
	let tabs = [
		{ name: 'Projects', link: '#projects' },
		{ name: 'About Me', link: '#about' }
	];
</script>

<header
	class={'sticky top-0 z-[10] flex items-center justify-between border border-solid px-6 duration-200' +
		(y > 0 ? ' border-emerald-950 bg-[#101010] py-4' : ' border-transparent bg-transparent py-6')}
>
	<h1>
		<b class="poppins text-2xl font-bold">Game Dev</b>
	</h1>
	<div class="flex items-center gap-8">
		<div class="hidden items-center gap-6 text-xl sm:flex">
			{#each tabs as tab}
				<a href={tab.link} class="duration-200 hover:text-emerald-600">
					<p>{tab.name}</p>
				</a>
			{/each}
		</div>
		<button
			class="text-l group relative overflow-hidden rounded-full bg-white px-5 py-2 text-slate-950 shadow-2xl shadow-emerald-600/90"
		>
			<div
				class="absolute right-full top-0 z-0 h-full w-full bg-emerald-600 opacity-30 duration-200 group-hover:translate-x-full"
			></div>
			<h4 class="z-9 relative">Contact Me</h4>
		</button>
	</div>
</header>
