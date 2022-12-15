<Layout>
    <div class="font-['DM_Serif_Display']"
    in:fade="{{duration:1000}}">
        <h1 class="text-center lg:text-2xl text-xl">Services</h1>
        <p class="text-center">We currently offer the following services:</p>
        <div class="flex flex-col gap-4 w-4/5 lg:w-1/5 m-auto">
            <div class="flex flex-row justify-between">
                <p>Cut, Blow and Dry</p>
                <p>£1.00</p>
            </div>
            <div class="flex flex-row justify-between">
                <p>Hair Coloring</p>
                <p>£1.00</p>
            </div>
            <div class="flex flex-row justify-between">
                <p>Hair Styling</p>
                <p>£1.00</p>
            </div>
            <div class="flex flex-row justify-between">
                <p>Other</p>
                <p>Call us</p>
            </div>
        </div>
        <CallToAction/>
    </div>
</Layout>

<script>
    import CallToAction from '../../components/call_to_action.svelte';
    import Layout from '../../components/layout.svelte';
    import {fade} from 'svelte/transition'
</script>