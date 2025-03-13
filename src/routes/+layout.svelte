<script>
  import Navigation from '$lib/Navigation.svelte';

  const links = [
    { href: '/temperature-converter', label: 'Temperature Converter' },
    { href: '/timer', label: 'Timer' },
    { href: '/circle-drawer', label: 'Circle Drawer' },
    { href: '/crud', label: 'CRUD' },
    { href: '/counter', label: 'Counter' },
    { href: '/cells', label: 'Cells' },
    { href: '/flight-booker', label: 'Flight Booker' }
  ];
</script>

<style>
  main {
    max-width: 100%;
    box-sizing: border-box;
  }
</style>

<Navigation {links} />
<slot />
