<script>
	export let name;
  import "./style/app.css";
	import Tailwindcss from './Tailwindcss.svelte';
  import Header from './Header.svelte';
</script>
<Tailwindcss/>


<Header/>
<main>
<p class="text-6xl font-bold underline rainbow-text">
	Hello {name}!
</p>

<p class='subscribe'>Subscribe My Youtube <a href="https://www.youtube.com/channel/UC4X8XQ6AMEHdVQOuMiEd5-A"><img alt='subscribe' src="/images/subcribe.png" class='inline-flex'/></a></p>


</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}
	.subscribe {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
  }
  .subscribe img {
height:50px;
}


.rainbow-text {
background-image: linear-gradient(to left, violet, indigo, blue, green, yellow, orange, red);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
 
  color: transparent;
} 

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
