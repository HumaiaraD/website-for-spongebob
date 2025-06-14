<script lang="js">
	import '../app.css';
	import Header from '../components/Header.svelte';
	import Footer from '../components/Footer.svelte';

	//let { children } = $props();
	let y;
	let innerHeight = 0;
	let innerWidth = 0;

</script>

<div class="relative flex flex-col max-w-[1400px] mx-auto w-full text-sm">
	<div class={"fixed botttom-0 w-full duration-200 flex p-10 z-[10] " + (
		y > 0 ? "opacity-full pointer-events-auto" : "pointer-events-none opacity-0"
	)}>
		<button on:click={goTop}
				class="ml-auto rounded-full bg-slate-900 text-yellow-400 px-3 sm:px-4 hover:bg-slate-50 cursor-pointer">
			<i class="fa-solid fa-arrow-up"/>
		</button>
	</div>
	<Header {y} {innerHeight}/>
	<slot />
	<Footer />
</div>

<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth />

<!--{@render children()}-->
