<script>
    import { footerLinks } from "$lib/index.js";

</script>

<section id="footer" class="mt-20 py-10 border-t border-neutral-700">
    <div class="flex sm:col-span-1 md:row-span-4 lg:col-span-4 justify-around">
       {#each footerLinks as footer}
            <div>
                <h2 class="text-md font-semibold mb-4">{footer.label}</h2>
                <ul class="space-y-2">
                    {#each footer.links as li}
                        <li class="text-neutral-300"><a href="/" class="hover:text-amber-100">{li}</a></li>
                    {/each}
                </ul>
            </div>
       {/each}
        <div class="flex flex-col gap-3">
            <span class="text-md font-semibold">Sign Up for Updates</span>
             <a href="/"><span class="py-2 px-4 border rounded-xl hover:bg-gradient-to-tr from-orange-500 to-orange-800">Sign Up</span></a>
        </div>
    </div>
</section>
