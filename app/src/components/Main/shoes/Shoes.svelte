<script>
    const bagDisplay = [
        {productPhoto: "/shoes/img1.jpg", productName: "Gold watch"},
        {productPhoto: "/shoes/img2.jpg", productName: "Hacks gold"},
        {productPhoto: "/shoes/img3.jpg", productName: "Palm rover"},
        {productPhoto: "/shoes/img4.jpg", productName: "Deem watch"},
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