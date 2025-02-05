<script>
  import { base } from "$app/paths";
  import Working from "$lib/working-link.svelte";
  import Broken from "$lib/broken-link.svelte";

  let { children } = $props();
</script>

<nav>
  <ul>
    <li><a href="{base}/">Home</a></li>
    <li>
      <Broken href="{base}/some/page">Some page (broken)</Broken>
    </li>
    <li>
      <Working href="{base}/some/page">Some page (working)</Working>
    </li>
  </ul>
</nav>

{@render children()}
