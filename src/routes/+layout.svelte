<script>
  import Navigation from '$lib/Navigation.svelte';

  const links = [
    { href: '/counter', label: 'Counter' },
    { href: '/temperature-converter', label: 'Temperature Converter' },
    { href: '/flight-booker', label: 'Flight Booker' },
    { href: '/timer', label: 'Timer' },
    { href: '/crud', label: 'CRUD' },
    { href: '/cells', label: 'Cells' },
    { href: '/circle-drawer', label: 'Circle Drawer' }
  ];
</script>


<Navigation {links} />
<slot />
