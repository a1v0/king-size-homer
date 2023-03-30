<script lang="ts">
    import Header from "./Header.svelte";
    import Footer from "./Footer.svelte";
    import Terminal from "./Terminal.svelte";

    export let name: string;
</script>

<Header />
<main>
    <h1>Hello {name}!</h1>
    <p>
        Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
        how to build Svelte apps.
    </p>
    <Terminal />
</main>
<Footer />
