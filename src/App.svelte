<script>
	import Header from './Header.svelte';
	import Opening from './Opening.svelte'
	import Introduction from './Introduction.svelte'
	import PaliPronunciation from './PaliPronunciation.svelte'
	import PaliAlphabet from './PaliAlphabet.svelte'
	import WordFormation from './WordFormation.svelte';
	
	const webpages = [
		{ name: "Opening", component: Opening },
		{ name: "Introduction", component: Introduction },
		{ name: "Pli Pronunciation", component: PaliPronunciation },
		{ name: "Pli Alphabet", component: PaliAlphabet },
		{ name: "Word Formation", component: WordFormation},
	];
	
	let index = 0
	$: selectedPage = webpages[index];
</script>


<article id="main-container-intro-grammar">
	<Header on:change={(e) => index = e.target.value} />
	<!-- Main Content -->
	<main id="main-content-ipg">
		<svelte:component this={selectedPage.component} />	
	</main>
</article>	