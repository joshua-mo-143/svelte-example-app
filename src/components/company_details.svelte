<div class="lg:col-span-1 font-['DM_Serif_Display'] text-center"
    in:fly="{{x:-500, duration:1000, delay: 300}}">
    <div class="text-left w-4/5 m-auto">
        <h1 class="text-center text-xl lg:text-2xl">Contact Details:</h1>
        <hr class="border-black my-5"/>
    <div class="flex flex-row gap-4">
        <img src="/phone-solid.svg" alt="Phone icon" height="20" width="20">
    <p>+44 12345 678901</p>
    </div>
    <div class="flex flex-row gap-4">
        <img src="/envelope-solid.svg" alt="Phone icon" height="20" width="20">
        <p>hello@loremipsum.com</p>
    </div>
    <hr class="border-black my-5"/>

    <p class="text-xl">Address:</p>
    <div class="ml-2">
        <p>123 Meme Road</p>
    <p>Meme Town</p>
    <p>Meme City</p>
    <p>Meme Country</p>
    <p>12345</p>
    </div>
    </div>
</div>

<script lang="ts">
    import {fly} from 'svelte/transition'
</script>