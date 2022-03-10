<script>
	import Header from './Header.svelte';
	import Opening from './Opening.svelte'
	import Introduction from './Introduction.svelte'
	import PaliPronunciation from './PaliPronunciation.svelte'
	import PaliAlphabet from './PaliAlphabet.svelte'
	import WordFormation from './WordFormation.svelte';
	import SimpleSentences from './SimpleSentences.svelte';
	import NounDeclension from './NounDeclension.svelte';
	import NounCompounds from './NounCompounds.svelte';
	import VerbConjugations from './VerbConjugations.svelte';
	
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

	];

	const menuOptions = components.reduce((allNames, currObj) => {
		return [...allNames, currObj.name]
	}, [])
	
	let index = 0
	$: selectedPage = components[index];
</script>


<article id="main-container-intro-grammar">
	<Header on:change={(e) => index = e.target.value} {menuOptions} />
	<!-- Main Content -->
	<main id="main-content-ipg">
		<svelte:component this={selectedPage.component} />	
	</main>
</article>	