<script lang="ts">
  import Header from './Header.svelte'
  import Footer from './Footer.svelte'

  import "./app.css";

  let { children } = $props();

</script>


<Header />
<!-- bg-[<value>] -->

<main class="space-y-8 bg-teal-100">
    {@render children()}
</main>

<Footer />
