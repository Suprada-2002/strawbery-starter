<script>
    import { navLinks } from "$lib/index.js";
    import Menu from "lucide-svelte/icons/menu";

    export let sideBar = false;

    function toggleSideBar() {
        sideBar = !sideBar;
    }

</script>
<div class="absolute top-0 left-0 w-full py-2 text-white z-20">
    <div data-aos="fade-down" class="container">
        <div class="flex justify-between items-center">
            <h1 class="text-4xl font-bold uppercase">
                Straw<span class="font-normal">Berries</span>
            </h1>
            <ul class="space-x-14 text-xl hidden lg:flex">
                {#each navLinks as links}
                    <li><a href={links.href}>{links.label}</a></li>
                {/each}
            </ul>
            <div onclick={toggleSideBar}>
                <Menu class="text-3xl cursor-pointer" />
            </div>
        </div>
    </div>
</div>
