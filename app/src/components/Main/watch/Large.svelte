<script>
    import Carousel from 'svelte-carousel';
    import { browser } from '$app/environment';

    let carousel;
  
    const handleNextClick = () => {
        carousel.goToNext()
    }

    const phoneDisplay = [
        {productPhoto: "/watch/img1.jpg", productName: "Gold watch"},
        {productPhoto: "/watch/img2.jpg", productName: "Hacks gold"},
        {productPhoto: "/watch/img3.jpg", productName: "Palm rover"},
        {productPhoto: "/watch/img4.jpg", productName: "Deem watch"},
    ]
</script>


<div class="mt-10">
    {#if browser}
  <Carousel
    bind:this={carousel}
  >
    {#each phoneDisplay as {productPhoto}}
        <div style="background-image: url({productPhoto})" class="bg-center bg-cover h-100"></div>
    {/each}
  </Carousel>
{/if}
</div>