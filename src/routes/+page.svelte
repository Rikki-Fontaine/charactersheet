<script>
	import Layout from "./+layout.svelte";
  	import Stats from "../components/stats.svelte";
  	import Portrait from "../components/portrait.svelte";
  	import Health from "../components/health.svelte";
  	import DeathSaves from "../components/deathSaves.svelte";
  	import Attacks from "../components/attacks.svelte";
</script>

<div class="flex-col justify-center mt-1 p-2">
	<Health/>
	<div class="flex md:justify-around justify-between p-2">
		<DeathSaves/>
		<Attacks/>
	</div>
	<Stats/>

</div>
<hr>
