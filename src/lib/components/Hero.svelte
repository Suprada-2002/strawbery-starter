<script>
    import Facebook from "lucide-svelte/icons/facebook";
    import Instagram from "lucide-svelte/icons/instagram";
    import Linkedin from "lucide-svelte/icons/linkedin";
    import Logo from "$lib/assets/strawberry.png";
    import Navbar from "./Navbar.svelte";

    let sideBar = false;

</script>

<main class="md:px-12 md:py-6 bg-primaryDark">
    <section class="relative min-h-[650px] bg-gradient-to-r from-primary to-secondary w-full md:rounded-xl shadow-md">
            <div class="container">

               <Navbar bind:sideBar/>
               
                 <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 place-items-center min-h-[665px]">

                     <div class="text-white mt-[100px] md:mt-0 p-4 space-y-4">

                         <h1 data-aos="fade-right" data-aos-delay="300" class="text-3xl pl-6 md:pl-14">01_____</h1>
                         <h1 data-aos="fade-up" class="text-5xl font-bold uppercase text-shadow">A healthy Fruit</h1>
                        <p data-aos="fade-up" data-aos-delay="300" class="text-sm">
                            Lorem ipsum dolor sit amet consectetur adipisicing elit.
                            Aspernatur soluta modi optio suscipit ex ipsum minus hic,
                            voluptates accusantium dolor!
                            </p>
                            <button data-aos="fade-up" data-aos-delay="500" class="border border-white px-4 py-2 rounded-lg">
                                Shop Now
                            </button>
                     </div>

                      <div>
                        <img src={Logo} alt="strawberry" class="img-shadow relative z-[1] w-[400px]" />
                    </div>


                    <div class="md:hidden"></div>


                 </div>
            </div>


        <h1 data-aos="zoom-out" class="text-center text-[80px] sm:text-[120px] md:text-[150px] xl:text-[180px] text-white uppercase font-bold absolute bottom-0 w-full z-0 text-shadow">
            berries
        </h1>


        {#if sideBar}
            <div class="absolute top-0 right-0 w-[120px] h-full bg-gradient-to-b from-primary to-secondary z-10">
                <div class="w-full h-full flex justify-center items-center">
                    <div class="text-white flex flex-col justify-center items-center gap-6">

                        <!-- line -->
                        <div class="w-[1px] h-[70px] bg-white"></div>

                        <div class="inline-block p-2 rounded-full cursor-pointer border border-white"><Facebook class="text-2xl" /></div>
                        <div class="inline-block p-2 rounded-full cursor-pointer border border-white"><Instagram class="text-2xl" /></div>
                        <div class="inline-block p-2 rounded-full cursor-pointer border border-white"><Linkedin class="text-2xl" /></div>

                        <div class="w-[1px] h-[70px] bg-white"></div>
                    </div>
                </div>
            </div>
        {/if}

    </section>
</main>




           

     
           
               
        
     

        
