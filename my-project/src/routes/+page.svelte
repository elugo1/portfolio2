<script>
  import Card from './../components/Card.svelte';

  const items = [
    {
      title: 'Pen Plots',
      imageUrl: '/thumbnail_images/project1.png',
      link: '/2024/a1'
    },
    {
      title: 'Where the Edge of Me Meets Another',
      imageUrl: '/thumbnail_images/project4.png',
      link: '/2024/a1'
    },
    {
      title: 'Microscope Panoramas',
      imageUrl: '/thumbnail_images/p7.png',
      link: '/2024/a1'
    },
    {
      title: 'Cemetery Spore Prints',
      imageUrl: '/thumbnail_images/mushroom_thumbnail.png',
      link: '/2024/a1'
    },
    {
      title: 'B☆A Revival',
      imageUrl: '/thumbnail_images/bstaraposter.png',
      link: '/2024/a1'
    }
  ];
</script>

<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 p-4">
{#each items as item}
  <Card title={item.title} imageUrl={item.imageUrl} link={item.link} />
{/each}
</div>
