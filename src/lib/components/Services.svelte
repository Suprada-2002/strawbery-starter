<script>
    import Logo from '$lib/assets/strawberry.png';
</script>

<section id="services" class="py-20">
    <div class="mb-16 text-center">
                <h1 data-aos="fade-up" data-aos-delay="300" class="text-3xl pl-6 md:pl-14">02_____</h1>
                <h1 data-aos="fade-up" class="text-5xl font-bold uppercase text-shadow">About Us</h1>
        </div>

    <div class="flex flex-col gap-5 p-2">

        <!-- card -1 -->
         <div class="lg:flex">
            <div class="md:shrink-0">
            <img src={Logo} alt="p-1" class="w-60 md:w-120 lg:300 object-cover md:h-full "/>
            </div>
            <div class="flex gap-3 flex-col p-10">
              <h2 class="text-3xl font-bold uppercase text-shadow">Juicy</h2>
              <p class="text-neutral-300">It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here, content here', making it look like readable English</p>
              <a href="/" ><span class="px-2 py-3 rounded-md bg-gradient-to-tr from-orange-500 to-orange-800">Know More__</span></a>
            </div>
         </div>

         <!-- card -2 -->
         <div class="lg:flex">
            
            <div class="flex gap-3 flex-col p-10">
                 <h2 class="text-3xl font-bold uppercase text-shadow">Tasty</h2>
                <p class="text-neutral-300">There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable.</p>
                <a href="/" ><span class="px-2 py-3 rounded-md bg-gradient-to-tr from-orange-500 to-orange-800">Know More__</span></a>
            </div>
            <div class="md:shrink-0">
            <img src={Logo} alt="p-2 " class="w-60 md:w-120 lg:300 object-cover md:h-full "/>
            </div>
         </div>

    </div>
</section>
