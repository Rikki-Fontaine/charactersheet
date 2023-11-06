<script>
	import '../app.postcss';
	import { AppShell } from '@skeletonlabs/skeleton';
	import Sidebar from "../components/sidebar.svelte";
	import Header from '../components/header.svelte';
	import Footer from '../components/footer.svelte';
  import Portrait from '../components/portrait.svelte';
</script>

<AppShell>
	<svelte:fragment slot="header">
		<Portrait/>

	</svelte:fragment>

	<svelte:fragment slot="sidebarLeft">
		<Sidebar>

		</Sidebar>
	
	</svelte:fragment>
	<!-- (sidebarRight) -->
	<!-- (pageHeader) -->
	<!-- Router Slot -->
	<slot />
	<!-- ---- / ---- -->
	
	<svelte:fragment slot="pageFooter">
		<Footer/>
	</svelte:fragment>
	<!-- (footer) -->

</AppShell>

