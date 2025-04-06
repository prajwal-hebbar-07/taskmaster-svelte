<script>
  const { children, ...props } = $props();
</script>

<button {...props}>{@render children()}</button>

<style>
  button {
    background-color: black;
    color: white;
    padding: 20px 24px;
    font-weight: normal;
    font-size: 22px;
    text-transform: uppercase;
    transition: all 0.3s;
  }

  button:hover {
    background-color: white;
    color: black;
  }
</style>
