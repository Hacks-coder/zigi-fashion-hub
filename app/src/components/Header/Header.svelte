<script>
    import IconMenu from '~icons/mdi/menu';
    import IconUser from '~icons/mdi/account';
    import IconCart from '~icons/mdi/cart';

    const logo = "/logo/logo.png"
</script>

<header class="@container flex justify-between text-2xl">
    <IconMenu />
    <div class="flex gap-1 items-center">
        <div class="size-6 rounded-full bg-cover bg-center" style="background-image: url({logo})"></div>
        <p class="font-bold text-xl @3xl:text-3xl">ZIGI FASHIOH HUB</p>
    </div>
    <div class="flex gap-2">
       <IconUser />
       <IconCart />
    </div>
</header>