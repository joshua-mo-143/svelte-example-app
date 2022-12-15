<div class="grid grid-cols-1 grid-rows-1 lg:grid-cols-2 overflow-hidden">
    <div class="col-span-1 flex flex-col justify-center items-center w-full h-[20rem] lg:h-[30rem] gap-4 lg:row-start-1 row-start-2"
    in:fly="{{x:-200, duration:1000}}">
        <h1 class="text-2xl text-stone-500 font-['DM_Serif_Display']">welcome to lorem ipsum</h1>
        <a href="/contact">
            <button class="text-xl bg-white text-black hover:text-white hover:bg-black transition-all px-5 py-2 rounded-xl font-['DM_Serif_Display']">book an appointment</button>
        </a>
    </div>
    <div class="flex flex-col justify-center items-center mt-5" in:fly="{{x:200, duration:1000}}">
        <img src="/header-img.webp" id="header-img" alt="Hairdresser cutting someone's hair" width="70%" height="100%" class="inline object-cover">
    </div>
</div>

<script>
        import { fly } from "svelte/transition";
</script>