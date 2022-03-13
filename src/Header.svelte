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
		<button id="prev-arrow" class="btn-arrow" on:click={() => dispatch('prev')}>&#8592;</button>
		
		<select on:change bind:value={index}>
			<option value="" disabled>Go to section:</option> 
				{#each menuOptions as linkName, i}
			<option value={i}>{linkName}</option>
			{/each}
		</select>
		
		<button id="next-arrow" class="btn-arrow" on:click={() => dispatch('next')}>&#8594;</button>
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
	

	button.btn-arrow {
		background-color: hsl(41, 36%, 20%);
		color: white;
		padding: 3px 5px 5px;
		font-size: 1.1rem;
		border-radius: 50%;
		cursor: pointer;
	}
	
	button.btn-arrow:active {
		background-color: hsl(22, 75%, 42%);
	}
</style>