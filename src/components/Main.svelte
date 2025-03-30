<style>
	@keyframes gradientShift {
		0% {
			background-position: 0% 50%;
		}
		50% {
			background-position: 100% 50%;
		}
		100% {
			background-position: 0% 50%;
		}
	}

	.animated-gradient {
		background-size: 200% 200%;
		animation: gradientShift 5s ease infinite;
	}
</style>

<main class="flex flex-col">
	<section
		id="introPage"
		class="flex items-center justify-center h-screen w-full text-center"
	>
		<div>
			<h2
				class="text-4xl font-semibold sm:text-5xl md:text-7xl lg:text-9xl leading-tight"
			>
				<span
					class="font-montserrat font-bold bg-gradient-to-r from-emerald-500 to-purple-800 inline-block text-transparent bg-clip-text animated-gradient"
				>
					JoinException
				</span>
			</h2>
			<a href="https://discord.com/users/713798379053908049"><button
				class="relative duration-500 font-bold mt-6 bg-[#1B1B1C] overflow-hidden rounded-2xl px-6 py-3 font-montserrat text-base text-white shadow-xl shadow-emerald-600/35 sm:text-md md:text-lg hover:bg-[#151516] hover:shadow-emerald-400/40"
			>
				<h4>Contact me ✌️</h4>
			</button></a>
		</div>
	</section>

	<section id="projects" class="flex flex-col items-center justify-center gap-8 py-14">
		<div class="text-center">
			<p class="font-montserrat text-base font-semibold sm:text-lg md:text-xl">My Projects</p>
			<p class="font-montserrat text-gray-500">A selection of projects I've worked on recently.</p>
		</div>
		<div class="grid h-fit grid-cols-1 gap-4">
			<div
				class="flex flex-col bg-[#0F0F10] duration-300 border border-neutral-700 hover:border-emerald-800 transition-all duration-300 items-center rounded-lg px-8 py-10 shadow-lg shadow-neutral-900/20"
			>
				<h3 class="font-montserrat text-lg font-semibold">Jammer</h3>
				<p class="font-montserrat text-sm text-gray-500">Wifi, Bluetooth & Car Jammer</p>
				<a href="https://github.com/Join-Exception/Wifi-BLE-Jammer">
					<button
						class="relative duration-500 font-bold mt-4 bg-[#1B1B1C] overflow-hidden rounded-2xl px-7 py-2 font-montserrat text-base text-white shadow-xl shadow-emerald-600/35 text-md hover:bg-[#151516] hover:shadow-emerald-400/35"
					>
						<h5>Github</h5>
					</button>
				</a>
			</div>

			<div
				class="flex flex-col bg-[#0F0F10] duration-300 border border-neutral-700 hover:border-emerald-800 transition-all duration-300 items-center rounded-lg px-8 py-10 shadow-lg shadow-neutral-900/20"
			>
				<h3 class="text-lg font-semibold">Servers</h3>
				<p class="text-sm text-gray-500">I am getting into Server & Networking stuff</p>
			</div>
			<div
			class="flex flex-col bg-[#0F0F10] duration-300 border border-neutral-700 hover:border-emerald-800 transition-all duration-300 items-center rounded-lg px-8 py-10 shadow-lg shadow-neutral-900/20"
		>
			<h3 class="text-lg font-semibold">Shop</h3>
			<p class="text-sm text-gray-500">I am currently coding an online shop(in progress)</p>
			<a href="https://shop.joinexception.de/">
			<button
			class="relative duration-500 font-bold mt-4 bg-[#1B1B1C] overflow-hidden rounded-2xl px-7 py-2 font-montserrat text-base text-white shadow-xl shadow-emerald-600/35 text-md hover:bg-[#151516] hover:shadow-emerald-400/35"
		>
			<h5>Check it out</h5>
		</button>
	</a>
		</div>
	</section>

	<section id="about" class="flex flex-col items-center justify-center gap-8 py-14">
		<div class="text-center">
			<p class="text-base font-semibold sm:text-lg md:text-xl">About Me</p>
			<div
				class="mt-6 flex flex-col bg-[#0F0F10] duration-300 border border-neutral-700 hover:border-emerald-800 transition-all duration-300 items-center rounded-lg px-8 py-10 shadow-lg shadow-neutral-900/20"
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
					I am a teenager getting into new technologies & I am <br> looking forward to new projects <br />
				</p>
			</div>
		</div>
	</section>
</main>
