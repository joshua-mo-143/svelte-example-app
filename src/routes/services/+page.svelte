<Layout>
    <div
    in:fade="{{duration:1000}}">
        <h1 class="text-center">Services</h1>
        <p class="text-center">We currently offer the following services:</p>
        <div class="flex flex-col gap-4 w-4/5 lg:w-1/5 m-auto">
            <div class="flex flex-row justify-between">
                <p>mem</p>
                <p>£1.25</p>
            </div>
            <div class="flex flex-row justify-between">
                <p>Cut, Blow and Dry</p>
                <p>£1.25</p>
            </div>
            <div class="flex flex-row justify-between">
                <p>Hair Coloring</p>
                <p>£1.25</p>
            </div>
            <div class="flex flex-row justify-between">
                <p>mem</p>
                <p>£1.25</p>
            </div>
        </div>
        <CallToAction/>
    </div>
</Layout>

<script>
    import CallToAction from '../../components/call_to_action.svelte';
    import Layout from '../../components/layout.svelte';
    import {fly, fade} from 'svelte/transition'
</script>