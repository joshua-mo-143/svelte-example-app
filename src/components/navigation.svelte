<nav class="h-20 text-3xl lg:text-5xl w-full flex flex-row justify-center lg:justify-start w-[90%] ml-3 overflow-hidden">
    <ul class="flex flex-row items-center justify-between lg:gap-10 gap-[8rem] text-gray-200 font-['DM_Serif_Display']">
        <li>
            <a href="/">
                <h1 class="navigation-title text-center drop-shadow-sm  hover:text-black transition-all">Lorem Ipsum.</h1>
            </a>
        </li>
        <li class="hidden lg:inline text-xl hover:text-black transition-all">
            <a href="/about">About</a>
        </li>
        <li class="hidden lg:inline text-xl hover:text-black transition-all">
            <a href="/services">Services</a>
        </li>
        <li class="hidden lg:inline text-xl hover:text-black transition-all">
            <a href="/contact">Contact</a>
        </li>
        <button on:click={handleToggle} class="lg:hidden">
            <img src="/bars-solid.svg" width="25px" height="25px" alt="Responsive menu icon"/>
        </button>
    </ul>
</nav>

{#if toggle == true}
    <div class="z-10 w-4/5 absolute top-0 right-0 h-screen bg-stone-500"
    in:fly="{{x:500, duration:500}}"  out:fly="{{x:500, duration:500}}">
        <button on:click={handleToggle}>
            <img src="/xmark-solid.svg" width="25px" height="25px" alt="Responsive menu icon" class="ml-4 mt-4">
        </button>
        <ul class="ml-5 mt-10 text-left text-2xl flex flex-col gap-4 font-['DM_Serif_Display']">
            <li class="hover:text-white transition-all">
                <a href="/about">
                    About
                </a>
            </li>
            <li class="hover:text-white transition-all">
                <a href="/services">
                    Services
                </a>
            </li>
            <li class="hover:text-white transition-all">
                <a href="/contact">
                    Contact
                </a>
            </li>
        </ul>
    </div>
{/if}

<script lang="ts">
    import {fly} from 'svelte/transition'

    let toggle: Boolean = false;

    const handleToggle = () => {
        toggle = !toggle;
    }
</script>