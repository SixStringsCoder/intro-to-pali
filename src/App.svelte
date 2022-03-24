<script>	
	import { onMount } from "svelte";

	import Nav from './Nav.svelte';
	import Footer from './Footer.svelte';	
	import Opening from './Opening.svelte'
	import Introduction from './Introduction.svelte'
	import PaliPronunciation from './PaliPronunciation.svelte'
	import PaliAlphabet from './PaliAlphabet.svelte'
	import WordFormation from './WordFormation.svelte';
	import SimpleSentences from './SimpleSentences.svelte';
	import NounDeclension from './NounDeclension.svelte';
	import NounCompounds from './NounCompounds.svelte';
	import VerbConjugations from './VerbConjugations.svelte';
	import AdjAndAdv from './AdjAndAdv.svelte';
	import Pronouns from './Pronouns.svelte';
	import Indeclinables from './Indeclinables.svelte';
	import Prefixes from './Prefixes.svelte';
	import Suffixes from './Suffixes.svelte';
	import Epilogue from './Epilogue.svelte';
	
	
	const components = [
		{ name: "Opening", component: Opening },
		{ name: "Introduction", component: Introduction },
		{ name: "Pāli Pronunciation", component: PaliPronunciation },
		{ name: "Pāli Alphabet", component: PaliAlphabet },
		{ name: "Word Formation", component: WordFormation },
		{ name: "Syntax: Simple Sentences", component: SimpleSentences },
		{ name: "Declension of nouns", component: NounDeclension },
		{ name: "Compounds of nouns", component: NounCompounds },
		{ name: "Conjugation of verbs", component: VerbConjugations },
		{ name: "Adjectives and adverbs", component: AdjAndAdv },
		{ name: "Pronouns (nāma)", component: Pronouns },
		{ name: "Indeclinables (nipāta)", component: Indeclinables },
		{ name: "Prefixes (upasagga)", component: Prefixes },
		{ name: "Suffixes", component: Suffixes },
		{ name: "Epilogue", component: Epilogue },

	];

	const menuOptions = components.reduce((allNames, currObj) => {
		return [...allNames, currObj.name]
	}, [])
	
	let index = 0
	let topOfPage;
	$: selectedPage = components[index];

	const goToPageTop = () => topOfPage.scrollIntoView();

	const handleMenu = (e) => {
		index = Number(e.target.value)
		goToPageTop();
	}

	const goToNext = () => {
		goToPageTop();
		if (index >= components.length-1) {
			return index = 0;
		}
		return index += 1;
	}
	
	const goToPrev = () => {
		goToPageTop();
		if (index === 0) {
			return index = components.length-1;
		}
		return index -= 1;
	}

	// Go to top of webpage whenever new component mounts
  onMount(() => goToPageTop());
	
</script>	


<header bind:this={topOfPage}>
	<h1 class="title-ipg">Introduction to Pali <br />Pronunciation and Grammar</h1>

	<Nav on:change={handleMenu} 
			 on:prev={goToPrev}
			 on:next={goToNext}
			 bind:index
			 {menuOptions} />
</header>

<article id="main-container-intro-grammar">

	<!-- Main Content -->
	<main id="main-content-ipg">
		<svelte:component this={selectedPage.component} />	
		<Nav on:change={handleMenu} 
			 on:prev={goToPrev}
			 on:next={goToNext}
			 bind:index
			 {menuOptions} />
	</main>

</article>	

<Footer />


<style>
	header {
		text-align: center;
		padding: 1rem 0.5rem;
		background-color: #ded2b9;
	}
	
	h1 {
		margin: 5px;
		font-size: 1.4rem
	}
	
</style>