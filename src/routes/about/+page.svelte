<Layout>
    <div class="grid lg:grid-rows-1 lg:grid-cols-2 grid-rows-2 grid-cols-1 mt-20 lg:mt-0 h-[45rem]">
        <div class="relative flex flex-col gap-4 justify-center items-center w-3/5 m-auto">
            <h1 class="text-3xl font-['DM_Serif_Display']" in:fade="{{duration: 500, delay:1000}}"
            on:mouseenter={handleMouseHover} on:mouseleave={handleMouseHover}
            >About Us...</h1>
        <p class="text-xl font-['Indie_Flower']" in:fade="{{duration: 500, delay:1000}}"
        on:mouseenter={handleMouseHover} on:mouseleave={handleMouseHover}
        >
            Hey there! We're a hair salon based in Rugeley, Staffordshire that caters to people who know the
             value of a good hairdresser that understands their needs. With our hairdressing expertise, we make sure that your haircut
            appointment leads to the result that you want, every single time. Check out some of our clients' reviews below...</p>
            <div id="about-front-card" class="-z-10 bg-stone-200 transition-all w-[110%] h-[120%] absolute rotate-[2deg] antialiased"
            in:fly="{{x:-500, duration: 500, delay:600}}"></div>
            <div class="-z-20 bg-stone-500 w-[110%] h-[120%] absolute rotate-[-2deg] antialiased"
            in:fly="{{x:-500, duration: 500, delay:200}}"
            ></div>
        </div>
        <div class="hidden lg:flex flex-col items-center justify-center">
            <img src="/about-img-1.webp" alt="" height="30%" width="50%" class="image object-cover relative" 
            in:fade="{{duration: 500, delay:1000}}">
        </div>
    </div>
<CustomerReviewSlider/>
    <CallToAction/>
</Layout>

<script lang="ts">
    import CallToAction from '../../components/call_to_action.svelte';
    import Layout from '../../components/layout.svelte';
    import { fly, fade } from "svelte/transition";
    import CustomerReviewSlider from '../../components/customer_review_slider.svelte';

    const handleMouseHover = () => {
        const frontcard = document.querySelector('#about-front-card');
        frontcard?.classList.toggle('bg-stone-200');
        frontcard?.classList.toggle('bg-white');
    }
</script>