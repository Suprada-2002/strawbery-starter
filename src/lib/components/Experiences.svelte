<script>

 import { testimonialData } from "$lib/index.js";
 import {onMount} from 'svelte';
 import { Swiper } from 'swiper';

 onMount(() => {
   var swiper = new Swiper(".mySwiper", {
        slidesPerView: 1,
        spaceBetween: 32,
        loop: true,
        centeredSlides: true,
        pagination: {
            el: ".swiper-pagination",
            clickable: true,

        },
        autoplay: {
            delay: 2500,
            disableOnInteraction: false,
        },
        breakpoints: {
        640: {
          slidesPerView: 1,
          spaceBetween: 32,
        },
        768: {
          slidesPerView: 2,
          spaceBetween: 32,
        },
        1024: {
          slidesPerView: 3,
          spaceBetween: 32,
        },
      },
    });

    });
</script>

<section class="py-24">
        <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
            <div class="mb-16 text-center">
                            <h1 data-aos="fade-up" data-aos-delay="300" class="text-3xl pl-6 md:pl-14">02_____</h1>
                         <h1 data-aos="fade-up" class="text-5xl font-bold uppercase text-shadow">Testimonial</h1>
                        <p data-aos="fade-up" data-aos-delay="300" class="text-sm">
                            Let's see what our user's say..
                            </p>
            </div>
            <!--Slider wrapper-->
            <div class="swiper mySwiper">
                <div class="swiper-wrapper w-max">
                
                    {#each testimonialData as data}

                    <div class="swiper-slide">
                        <div
                            class="group bg-white border border-solid border-white rounded-xl p-6 transition-all duration-500  w-full mx-auto hover:border-indigo-600 hover:shadow-sm slide_active:border-indigo-600">
                            <div class="">
                                <div class="flex items-center mb-7 gap-2 text-amber-500 transition-all duration-500  ">
                                    <svg class="w-5 h-5" viewBox="0 0 18 17" fill="none"
                                        xmlns="http://www.w3.org/2000/svg">
                                        <path
                                            d="M8.10326 1.31699C8.47008 0.57374 9.52992 0.57374 9.89674 1.31699L11.7063 4.98347C11.8519 5.27862 12.1335 5.48319 12.4592 5.53051L16.5054 6.11846C17.3256 6.23765 17.6531 7.24562 17.0596 7.82416L14.1318 10.6781C13.8961 10.9079 13.7885 11.2389 13.8442 11.5632L14.5353 15.5931C14.6754 16.41 13.818 17.033 13.0844 16.6473L9.46534 14.7446C9.17402 14.5915 8.82598 14.5915 8.53466 14.7446L4.91562 16.6473C4.18199 17.033 3.32456 16.41 3.46467 15.5931L4.15585 11.5632C4.21148 11.2389 4.10393 10.9079 3.86825 10.6781L0.940384 7.82416C0.346867 7.24562 0.674378 6.23765 1.4946 6.11846L5.54081 5.53051C5.86652 5.48319 6.14808 5.27862 6.29374 4.98347L8.10326 1.31699Z"
                                            fill="currentColor" />
                                    </svg>
                                    <span class="text-base font-semibold text-indigo-600">{data.num}</span>
                                </div>
                                <p
                                    class="text-base text-gray-600 leading-6  transition-all duration-500 pb-8 group-hover:text-gray-800 slide_active:text-gray-800">
                                    {data.text}
                                </p>
                            </div>
                            <div class="flex items-center gap-5 border-t border-solid border-gray-200 pt-5">
                                <img class="rounded-full h-10 w-10 object-cover" src={data.img}
                                    alt="avatar" />
                                <div class="block">
                                    <h5 class="text-gray-900 font-medium transition-all duration-500  mb-1">{data.name}</h5>
                                    <span class="text-sm leading-4 text-gray-500">{data.occupation} </span>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                {/each}
             
                </div>
                <div class="swiper-pagination text-white">* * *</div>
            </div>
        </div>
    </section>

<style>
        .swiper-horizontal>.swiper-pagination-bullets .swiper-pagination-bullet,
        .swiper-pagination-horizontal.swiper-pagination-bullets .swiper-pagination-bullet {
            width: 16px;
            height: 4px;
            border-radius: 5px;
            margin: 0 6px;
            text-align: center;
        }

        .swiper-pagination {
            bottom: 2px;
            color: white;
            text-align: center;
        }

        .swiper-wrapper {
            height: max-content;
            width: max-content;
            padding-bottom: 64px;
        }

        .swiper-pagination-bullet-active {
            background: white !important;
        }
        
        .swiper-slide.swiper-slide-active>.slide_active\:border-indigo-600 {
            --tw-border-opacity: 1;
            border-color: rgb(79 70 229 / var(--tw-border-opacity));
        }

        .swiper-slide.swiper-slide-active>.group .slide_active\:text-gray-800 {
            ---tw-text-opacity: 1;
            color: white;
            /* color: rgb(31 41 55 / var(--tw-text-opacity)); */
        }
    </style>
