<script>
    export let reviewItem;
    export let left;
    export let index;
</script>

<div class={"flex flex-col gap2 w-full max-w-[500px] mx-auto relative" + (
    left 
    ? index % 2 === 1 
        ? 'hidden md:flex opacity-0 pointer-events-none max-h-[40px] overflow-hidden' 
        : ' ' 
    : index % 2 === 0 
        ? 'hidden md:flex opacity-0 pointer-events-none max-h-[40px] overflow-hidden' 
        : ' '
)}
>
    <div class="flex relative">
        <div class={"absolute rounded-full bg-white aspect-square hidden md:grid place-items-center h-4 top-0 " + (index % 2 === 0 ? ' right-0 -mr-8 translate-x-1/2' : ' left-0 -ml-8 -translate-x-1/2')}
        >
            <div class="rounded-full bg-slate-950 h-2" />
        </div>
        <div class="flex items-center gap-2">
            <i></i>
        </div>
    </div>
</div>