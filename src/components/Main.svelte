<script>
	let fontCustom =
		'font-montserrat bg-gradient-to-r from-emerald-500 to-purple-500 inline-block text-transparent bg-clip-text';
</script>

<main class="flex flex-1 flex-col p-4">
	<section id="introPage" class="grid min-h-screen grid-cols-1 gap-10 py-8 sm:py-14 lg:grid-cols-2">
		<div
			class="flex flex-col justify-center gap-6 text-center md:gap-8 lg:justify-center lg:gap-10 lg:text-left"
		>
			<h2 class="text-4xl font-semibold sm:text-5xl md:text-6xl">
				Hi I'm <span class="{fontCustom} to-purple-800">JoinException</span> Developer & Pentester
			</h2>
			<p class="font-montserrat text-base sm:text-lg md:text-xl">
				My favorite programming language is <span class={fontCustom}>java</span> and I am a
				<span class={fontCustom}>grayhat</span>
			</p>
			<button
				class="relative font-bold mx-auto bg-[#0165D8] overflow-hidden rounded-2xl px-6 py-3 font-montserrat text-base text-white shadow-xl shadow-blue-600/35 sm:text-md md:text-lg lg:ml-0 lg:mr-auto"
			>
				<h4 class="z-9 relative">Contact me &rarr;</h4>
			</button>
		</div>
		<div class="flex items-center justify-center lg:justify-end">
			<img src="assets/logo.jpg" alt="Logo" class="h-[650px] max-w-full" />
		</div>
	</section>

	<section id="projects" class="flex flex-col items-center justify-center gap-8 py-14">
		<div class="text-center">
			<p class="font-montserrat text-base font-semibold sm:text-lg md:text-xl">My Projects</p>
			<p class="font-montserrat text-gray-500">A selection of projects I've worked on recently.</p>
		</div>
		<div class="flex flex-wrap justify-center gap-5">
			<div
				class="flex flex-col items-center rounded-xl border border-solid border-emerald-950 px-8 py-10 shadow-md"
			>
				<h3 class="font-montserrat text-lg font-semibold">Jammer</h3>
				<p class="font-montserrat text-sm text-gray-500">Wifi, Bluetooth & Car Jammer</p>
				<a href="https://github.com/Join-Exception/Wifi-BLE-Jammer">
					<button
						class="md:text-m group relative top-2 mx-auto overflow-hidden rounded-full bg-white px-6 py-3 font-montserrat text-slate-950 shadow-xl shadow-emerald-600/30 duration-500 hover:bg-slate-300 sm:text-lg lg:ml-0 lg:mr-auto"
					>
						<p>Github</p>
					</button>
				</a>
			</div>

			<div
				class="flex flex-col items-center rounded-xl border border-solid border-emerald-950 px-8 py-10 shadow-md"
			>
				<h3 class="text-lg font-semibold">Servers</h3>
				<p class="text-sm text-gray-500">I am getting into Server & Networking stuff</p>
			</div>
		</div>
	</section>
	<section id="about" class="flex flex-col items-center justify-center gap-8 py-14">
		<div class="text-center">
			<p class="text-base font-semibold sm:text-lg md:text-xl">About Me</p>
			<div
				class="mt-8 flex flex-col items-center rounded-xl border border-solid border-emerald-950 px-16 py-10 shadow-md"
			>
				<h3 class="flex items-center gap-2 font-montserrat text-lg font-semibold">
					I am from Germany
					<img
						src="https://upload.wikimedia.org/wikipedia/en/b/ba/Flag_of_Germany.svg"
						alt="Germany Flag"
						class="h-4 w-6"
					/>
				</h3>
				<p class="font-montserrat text-sm text-gray-500">
					I am a teenager getting into new technologies & i am <br />
				</p>
			</div>
		</div>
	</section>
</main>
