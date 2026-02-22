<script>
  // Import all SVGs from a folder using Vite's import.meta.glob
  const svgModules = import.meta.glob('/src/figmaAssets/Books/*.svg', {
    eager: true,
    query: '?url',
    import: 'default'
  });

  const svgFiles = Object.entries(svgModules).map(([path, url]) => ({
    url,
    name: path.split('/').pop().replace('.svg', '')
  }));

  export let imgClass = 'booksItem';
</script>

{#each svgFiles as { url, name }}
  <img
    src={url}
    alt={name}
    class={imgClass}
  />
{/each}

<style>
    .booksItem {
      border: 0.1px solid rgb(200, 200, 200);
        width: 12.5vw;
    }
</style>