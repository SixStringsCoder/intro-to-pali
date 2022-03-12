<script>
	import { createEventDispatcher } from 'svelte';

	const dispatch = createEventDispatcher();

  export let menuOptions = [];
	export let index;
</script>


<header>
	<!-- Title of Document -->	
	<h1 class="title-ipg">Introduction to Pali <br />Pronunciation and Grammar</h1>
	
	<nav class="custom-select">
		<div id="prev-arrow" class="arrows" on:click={() => dispatch('prev')}>&#10132;</div>
		
		<select on:change bind:value={index}>
			<option value="" disabled>Go to section:</option> 
				{#each menuOptions as linkName, i}
			<option value={i}>{linkName}</option>
			{/each}
		</select>
		
		<div id="next-arrow" class="arrows" on:click={() => dispatch('next')}>&#10132;</div>
	</nav>

	
</header>	


<style>
	header {
		text-align: center;
		padding: 1rem 0.5rem;
		background-color: #ded2b9;
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
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	.arrows {
		font-size: 1.5rem;
		cursor: pointer;
	}
	
	div#prev-arrow {
		transform: rotate(180deg)
	}
</style>