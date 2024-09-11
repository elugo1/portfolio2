  <script>
    import Card from '../../components/Card.svelte';
  
    const items = [
      {
        title: 'Project 1',
        imageUrl: '/images/project1.png',
        link: '/2024/a1'
      },
      {
        title: 'Project 1',
        imageUrl: '/images/project1.png',
        link: '/2024/a1'
      },
      {
        title: 'Project 1',
        imageUrl: '/images/project2.jpeg',
        link: '/2024/a1'
      },
      {
        title: 'Project 1',
        imageUrl: '/images/project1.png',
        link: '/2024/a1'
      }
    ];
  </script>
  
  <div class="grid grid-cols-3 sm:grid-cols-2 md:grid-cols-3 gap-4 p-7">
    {#each items as item}
      <Card title={item.title} imageUrl={item.imageUrl} link={item.link} />
    {/each}
  </div>
  