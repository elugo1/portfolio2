<script>
  import Card from './../components/Card.svelte';

  const items = [
    {
      title: 'Pen Plots',
      imageUrl: '/thumbnail_images/project1.png',
      link: '/Projects/plots'
    },
    {
      title: 'Where the Edge of Me Meets Another',
      imageUrl: '/thumbnail_images/project4.png',
      link: '/Projects/physarum'
    },
    {
      title: 'Microscope Panoramas',
      imageUrl: '/thumbnail_images/p7.png',
      link: '/Projects/panoramas'
    },
    {
      title: 'Cemetery Spore Prints',
      imageUrl: '/thumbnail_images/mushroom_thumbnail.png',
      link: '/Projects/mushrooms'
    },
    {
      title: 'B☆A Revival',
      imageUrl: '/thumbnail_images/bstaraposter.png',
      link: '/Projects/bstara'
    },
    {
      title: 'Silhouette Extractor',
      imageUrl: '/thumbnail_images/silhouette_extractor_1.png',
      link: '/Projects/silhouette'
    }
  ];
</script>

<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 p-4">
{#each items as item}
  <Card title={item.title} imageUrl={item.imageUrl} link={item.link} />
{/each}
</div>
