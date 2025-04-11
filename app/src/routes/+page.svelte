<script>
	import Large from './../components/Main/watch/Large.svelte';
	import Phone from './../components/Main/phone/Phone.svelte';
	import Bag from "../components/Main/bags/Bag.svelte";
	import MaleShirt from "../components/Main/shirt/MaleShirt.svelte";
	import Shoes from "../components/Main/shoes/Shoes.svelte";
import Small from "../components/Main/watch/Small.svelte";

</script>


<div class="@container">
    <Large />
    <Small />
     <div class="bg-red p-2 text-white font-bold text-center mt-10 @3xl:p-5">
        <p class="text-xl @3xl:text-2xl">FLASH SALE</p>
    </div>
    <Bag />
    <Phone />
    <div class="bg-red p-2 text-white font-bold text-center mt-10 @3xl:p-5">
        <p class="text-xl @3xl:text-2xl">QUALITY MAILE CLOTHING</p>
    </div>
    <MaleShirt />
    <Shoes />
</div>