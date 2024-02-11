<script>
    export let cls
    export let text
    export let base = 0

    function click() {
        switch (text) {
            case 'C':
                base = 0
                break
            default:
                base = text
        }
    }
    
    let f = cls + "text-white text-2xl bg-teal-900 rounded-full h-[10vh] w-[10vh] my-1 mx-1"
</script>
<button class={f} on:click={click}>{text}</button>
