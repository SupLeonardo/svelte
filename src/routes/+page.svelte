<script>
    import '../app.css'
    import Button from '../components/Button.svelte';
    export let name = 'Lev';
    let base = 0
</script>

<div class="items-center justify-center flex">
    <div class="">
        <h1 class="text-white text-6xl pb-5 pr-5 justify-end flex font-bold">{base}</h1>
        <div class="w-full flex justify-center">
            <Button cls='active:bg-sky-500 bg-sky-900' text='C'/>
            <Button cls='active:bg-sky-500 bg-sky-900' text='%'/>
            <Button cls='active:bg-sky-500 bg-sky-900' text='⌫'/>
            <Button cls='active:bg-sky-500 bg-sky-900' text='/'/></div>
    
            <div class="w-full flex justify-center">
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=7/>
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=8/>
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=9/>
            <Button cls='active:bg-sky-500 bg-sky-900' text='X'/></div>
    
            <div class="w-full flex justify-center">
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=4/>
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=5/>
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=6/>
            <Button cls='active:bg-sky-500 bg-sky-900' text='—'/></div>
    
            <div class="w-full flex justify-center">
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=1/>
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=2/>
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=3/>
            <Button cls='active:bg-sky-500 bg-sky-900' text='+'/></div>
    
            <div class="w-full flex justify-center">
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=0/>
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=00/>
            <Button cls='bg-emerald-700 active:bg-emerald-500' text=','/>
            <Button cls='active:bg-sky-500 bg-sky-900' text='='/></div>
    </div>
</div>