<template>
  <div>
    <OluFooter :links="links">
      Copyright © {{ new Date().getFullYear() }} <a href="https://www.kevin-custer.com/" target="_blank" class="font-bold text-green-700 hover:text-green-800" rel="noopener">Kevin Custer</a>. All rights reserved.
    </OluFooter>
  </div>
</template>

<script>
  export default {
    data: () => ({
      links: [
        { 
          label: 'RSS',
          url: '/rss.xml'
        },
        {
          label: 'Sitemap',
          url: '/sitemap.xml'
        }
      ]
    }),
  }
</script>
