<Layout>
<div class="grid lg:grid-cols-3 lg:grid-rows-1 grid-cols-1 grid-rows-2 lg:mt-20 overflow-hidden">
    <CompanyDetails/>
    <ContactForm/>
</div>
</Layout>

<script lang="ts">
    import ContactForm from '../../components/contact_form.svelte';
    import CompanyDetails from '../../components/company_details.svelte';
    import Layout from '../../components/layout.svelte';
</script>