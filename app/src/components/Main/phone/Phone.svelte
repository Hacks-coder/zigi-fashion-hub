<script>
    import Carousel from 'svelte-carousel';
    import { browser } from '$app/environment';

    let carousel;
  
    const handleNextClick = () => {
        carousel.goToNext()
    }

    const phoneDisplay = [
        {productPhoto: "/phones/img1.jpg", productName: "Gold watch"},
        {productPhoto: "/phones/img2.jpg", productName: "Hacks gold"},
        {productPhoto: "/phones/img3.jpg", productName: "Palm rover"},
        {productPhoto: "/phones/img4.jpg", productName: "Deem watch"},
    ]
</script>


<div class="mt-10">
    {#if browser}
  <Carousel
    bind:this={carousel}
  >
    {#each phoneDisplay as {productPhoto, productName}}
        <div style="background-image: url({productPhoto})" class="bg-center bg-cover size-50"></div>
    {/each}
  </Carousel>
{/if}

<button on:click={handleNextClick}>Next</button>
</div>