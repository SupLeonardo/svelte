<script>
    export let logo
</script>
<div class=" border-stone-200 rounded-xl w-[32%] flex justify-center mt-8 shadow-sm p-2 h-[45%] border-2 hover:bg-stone-300 ">
    {#if logo === 'apple'}
        <img width="50" height="50" src="https://img.icons8.com/ios-filled/50/mac-os.png" alt="mac-os"/>
    {:else if logo === 'google'}
        <img width="48" height="48" src="https://img.icons8.com/fluency/48/google-logo.png" alt="google-logo"/>
    {:else if logo === 'microsoft'}
        <img width="48" height="48" src="https://img.icons8.com/color/48/microsoft.png" alt="microsoft"/>
    {/if}
</div>