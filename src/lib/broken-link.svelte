<script>
  let { children, href, ...restProps } = $props();
</script>

<a {href} {...restProps}>
  {@render children?.()}
</a>
