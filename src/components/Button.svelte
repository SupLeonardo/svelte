<script>
    export let logo
</script>
<div class=" border-stone-200 rounded-xl w-[25%] mx-[1%] flex justify-center mt-8 shadow-sm  h-[35%] border-2">
    {#if logo === 'apple'}
        <img width="50" height="50" src="https://img.icons8.com/ios-filled/50/mac-os.png" alt="mac-os"/>
    {:else if logo === 'google'}
        <img width="48" height="48" src="https://img.icons8.com/fluency/48/google-logo.png" alt="google-logo"/>
    {:else if logo === 'microsoft'}
        <img width="48" height="48" src="https://img.icons8.com/color/48/microsoft.png" alt="microsoft"/>
    {/if}
</div>