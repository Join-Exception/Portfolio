<script>
	import { onMount } from 'svelte';

	let song = 'Music';
	let isPlaying = false;
	let audio;
	let volume = 0.1;

	onMount(() => {
		audio = new Audio('/assets/song.mp3');
		audio.volume = volume;
	});

	function togglePlay() {
		if (isPlaying) {
			audio.pause();
		} else {
			audio.play();
		}
		isPlaying = !isPlaying;
	}

	function changeVolume(event) {
		volume = event.target.value;
		if (audio) {
			audio.volume = volume;
		}
	}
</script>

<div
	class="music-player bottom-[10px] flex h-[160px] w-[200px] flex-col items-center justify-between rounded-xl border border-solid border-emerald-950 bg-black text-white"
>
	<p class="mt-5 font-montserrat">{song}</p>
	<div class="top-50 flex items-center justify-center">
		<button
			class="h-12 w-12 rounded-full bg-blue-500 focus:outline-none"
			on:click={togglePlay}
			aria-label={isPlaying ? 'Pause song' : 'Play song'}
		>
			<i class={`fa ${isPlaying ? 'fa-pause' : 'fa-play'} fa-2x text-white`} id="play-btn"></i>
		</button>
	</div>

	<div class="mb-2 w-full px-2 text-center">
		<label for="volume-slider" class="font-montserrat text-sm">Volume</label>
		<input
			id="volume-slider"
			type="range"
			min="0"
			max="1"
			step="0.01"
			value={volume}
			on:input={changeVolume}
			class="mt-2 w-full"
		/>
	</div>
</div>

<style>
	input[type='range'] {
		-webkit-appearance: none;
		width: 100%;
		height: 4px;
		background: #ddd;
		border-radius: 10px;
	}

	input[type='range']::-webkit-slider-thumb {
		-webkit-appearance: none;
		width: 20px;
		height: 20px;
		background: #0073e6;
		border-radius: 50%;
		cursor: pointer;
	}

	input[type='range']::-moz-range-thumb {
		width: 20px;
		height: 20px;
		background: #0073e6;
		border-radius: 50%;
		cursor: pointer;
	}

	@media (max-width: 768px) {
		.music-player {
			display: none;
		}
	}
</style>
