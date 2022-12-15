<div class="lg:col-span-2 row-span-1"
    in:fly="{{x:500, duration:1000, delay:300}}">
    <h1 class="text-center text-xl lg:text-2xl font-['DM_Serif_Display']">Contact Us</h1>
    <form action="" class="flex flex-col gap-4 items-center justify-center py-5">
        <p class="font-['DM_Serif_Display']">* = required</p>
        <label for="" class="flex flex-row justify-between gap-2 lg:w-2/5 items-center">
            <span class="font-['DM_Serif_Display']">Name*:</span>
            <input type="text" name="" class="w-4/5 px-2 py-1"/>
        </label>
        <label for="" class="flex flex-row justify-between gap-2 lg:w-2/5 items-center">
            <span class="font-['DM_Serif_Display']">Email*:</span>
            <input type="text" name="" class="w-4/5 px-2 py-1"/>
        </label>
        <label for="" class="flex flex-row justify-between gap-2 lg:w-2/5 items-center">
            <span class="font-['DM_Serif_Display']">Phone:</span>
            <input type="text" name="" class="w-4/5 px-2 py-1"/>
        </label>
        <label for="" class="flex flex-col lg:flex-row justify-between gap-2 lg:w-2/5 w-4/5 items-center">
            <span class="font-['DM_Serif_Display']">Message*:</span>
            <textarea name="" class="w-full h-20 px-2 py-1"/>
        </label>
        <button class="bg-stone-200 px-5 py-2 font-['DM_Serif_Display']">Send Message</button>
    </form>
</div>

<script>
    import {fly} from 'svelte/transition'
</script>