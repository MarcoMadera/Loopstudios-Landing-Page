<script>
	import Hero from "./components/Hero.svelte"
	import History from "./components/History.svelte"
	import Creations from "./components/Creations.svelte"
	import Footer from "./components/Footer.svelte"
</script>

<main>
	<Hero/>
	<div class="separator">
		<History/>
		<Creations/>
	</div>
	<Footer/>
</main>

<style>
	.separator{
		margin: 85px 24px;
	}
	@media screen and (min-width: 1024px){
		.separator {
			margin: 85px 160px;
		}
	}
</style>