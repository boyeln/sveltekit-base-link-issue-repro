<script>
  let { children, href } = $props();
</script>

<a {href}>
  {@render children?.()}
</a>
