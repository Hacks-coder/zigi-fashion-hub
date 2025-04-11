<script>

    const watchDisplay = [
        {productPhoto: "/watch/img1.jpg", productName: "Gold watch"},
        {productPhoto: "/watch/img2.jpg", productName: "Hacks gold"},
        {productPhoto: "/watch/img3.jpg", productName: "Palm rover"},
        {productPhoto: "/watch/img4.jpg", productName: "Deem watch"},
    ]
</script>

<div class="@container mt-10">
    <div class="grid grid-cols-2 gap-2 @3xl:grid-cols-4">
        {#each watchDisplay as {productPhoto, productName}}
            <div class="bg-cover bg-center h-50 rounded-xl flex items-end justify-center font-bold" style="background-image: url({productPhoto});">
                <p class="text-white text-center">{productName}</p>
            </div>
        {/each}
    </div>
</div>


<style>
    
</style>