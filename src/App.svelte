<script>
	import Navbar from './components/Navbar.svelte';
	import Header from './components/Header.svelte';
	import Projects from './components/Projects.svelte';
	import AOS from 'aos';
	import 'aos/dist/aos.css';
	import { onMount } from 'svelte';

	onMount(() => {
		AOS.init({
			duration: 1800,
			once: true
		});
	});
</script>

<svelte:head>
	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" />
</svelte:head>

<Navbar />
<Header />
<Projects />
