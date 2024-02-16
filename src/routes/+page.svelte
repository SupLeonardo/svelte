<script>
    import '../app.css'
    import Button from '../components/Button.svelte';
    export let name = 'Lev';
    let base = 0
</script>

<div class=" flex flex-col h-[80vh] w-[35vw] bg-white rounded-xl shadow-xl columns-1 items-center ">
    <img class=' h-[7vh] w-[7vh] mt-[2vh] ' src="https://img.icons8.com/ios/50/verified-account.png" alt="verified-account"/> <br />
    <h1 class=" flex justify-center font-bold w-[20vw] text-4xl ">Welcome back</h1>
    <h2 class=" mt-[1vh] text-2xl ">Please enter your details to sign in</h2>
    <div class=" w-full h-[20%] flex justify-center">
        <Button logo='apple' />
        <Button logo='google' />
        <Button logo='microsoft' />
    </div>
</div>