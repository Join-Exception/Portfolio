<script>
	import Footer from '../components/Footer.svelte';
	import Header from '../components/Header.svelte';
	import MusicPlayer from '../components/MusicPlayer.svelte';
	import '../app.css';
	import '@fontsource-variable/montserrat';
	let y;
	let innerWidth = 0;
	let innerHeight = 0;

	function goTop() {
		document.body.scrollIntoView();
	}
</script>

<!-- Render the regular page layout -->
<Header {y} {innerHeight} />
<div
	class="container relative mx-auto flex min-h-screen w-full max-w-[1400px] flex-col text-sm sm:text-base"
>
	<div
		class={'fixed bottom-0 z-[10] flex w-full p-10 duration-200 ' +
			(y > 0 ? ' opacity-full pointer-events-auto' : ' pointer-events-none opacity-0')}
	>
		<button
			on:click={goTop}
			class="ml-auto grid aspect-square cursor-pointer place-items-center rounded-full bg-emerald-900 px-3 text-white hover:bg-emerald-950 sm:px-4"
		>
			<i class="fa-solid fa-arrow-up" />
		</button>
	</div>
	<!--<Header {y} {innerHeight} /> -->
	<slot />
	<Footer />
</div>
<!--<MusicPlayer />-->

<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth />
