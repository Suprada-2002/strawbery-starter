<script>
    import '../app.css';
    import {onMount} from 'svelte';
    import 'aos/dist/aos.css';
    import AOS from 'aos';
    
    import Navbar from '$lib/components/Navbar.svelte';

    onMount(() => {
         AOS.init({
      offset: 100,
      duration: 800,
      easing: "ease-in-sine",
      delay: 100,
    });
    AOS.refresh();
    })
</script>

<slot />
