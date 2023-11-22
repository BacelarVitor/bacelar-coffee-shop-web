<script lang="ts">
    import '../app.css'
    import Header from '$lib/components/Header.svelte'
</script>

<main class="container">
    <Header />
    <slot/>
</main>