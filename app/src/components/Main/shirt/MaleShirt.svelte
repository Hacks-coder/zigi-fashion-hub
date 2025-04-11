<script>
    const bagDisplay = [
        {productPhoto: "/shirts/img1.webp", productName: "Gold watch"},
        {productPhoto: "/shirts/img2.webp", productName: "Hacks gold"},
        {productPhoto: "/shirts/img3.webp", productName: "Palm rover"},
        {productPhoto: "/shirts/img4.webp", productName: "Deem watch"},
    ]
</script>

<div class="@container mt-10">
    <div class="grid grid-cols-2 gap-2 mt-5 @3xl:grid-cols-4">
        {#each bagDisplay as {productPhoto, productName}}
            <div class="bg-cover bg-center h-50 rounded-xl flex items-end justify-center font-bold" style="background-image: url({productPhoto});">
                <p class="text-white text-center">{productName}</p>
            </div>
        {/each}
    </div>
</div>