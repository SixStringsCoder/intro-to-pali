<script>
  // export const lessonNames = [];
	// $: lessonLinks = lessonNames.filter(obj => obj.name)
	// $: console.log(lessonLinks)

	const lessonLinks = [
		"Opening", "Introduction", "Pāli Pronunciation", "Pāli Alphabet", "Word Formation", "Syntax: Simple Sentences", "Declension of nouns"
	];

</script>


<header>
	<!-- Title of Document -->	
	<h1 class="title-ipg">Introduction to Pali <br />Pronunciation and Grammar</h1>
	
	<nav class="custom-select">
		<select on:change>
			<option value="" disabled>Go to section:</option> 
				{#each lessonLinks as linkName, i}
					<option value={i}>{linkName}</option>
				{/each}
		</select>
	</nav>
</header>	


<style>
	header {
		text-align: center;
		padding: 1rem 0.5rem;
		background-color: #dcd3c0;
	}
	
	h1 {
		margin: 5px;
	}
	
	h1 {
		font-size: 1.4rem
	}
	
	
	nav {
		margin: 10px 0 0 0 ;
		padding: 0;
	}
	
</style>