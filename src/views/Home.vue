<template>
  <div id="home">
    <articles>
      <banner />
    </articles>

    <bannerSecond />

    <about />

  </div>
</template>

<script>
  export default {
    name: 'Home',

    components: {
      About: () => import('@/components/home/About'),
      Articles: () => import('@/components/home/Articles'),
      Banner: () => import('@/components/home/Banner'),
      BannerSecond: () => import('@/components/home/BannerSecond'),
      Social: () => import('@/components/home/Social'),
      Subscribe: () => import('@/components/home/Subscribe'),
    },
  }
</script>
