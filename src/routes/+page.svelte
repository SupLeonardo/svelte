<script>
    import '../app.css'
    import Button from '../components/Button.svelte';
    export let name = 'Lev';
    let base = 0
    
</script>

<div class=" flex flex-col h-[85vh] w-[80vw] lg:w-[50vw] sm:w-[65vw] bg-white rounded-xl shadow-xl columns-1 items-center px-[10%] ">
    <img class=' h-[7vh] w-[7vh] mt-[2vh] ' src="https://img.icons8.com/ios/50/verified-account.png" alt="verified-account"/> <br />
    <h1 class=" flex justify-center font-bold w-[45vw] xl:w-[20vw] text-4xl ">Welcome back</h1>
    <h2 class=" mt-[1vh] text-2xl ">Please enter your details to sign in</h2>
    <div class=" w-full h-[20%] flex justify-between">
        <Button logo='apple' />
        <Button logo='google' />
        <Button logo='microsoft' />
    </div>
    
    <div class="bg-[#ebebeb] w-full h-1 flex justify-center ">
        <div class=" mt-[-2%] w-[10%] bg-white flex justify-center">
            <h1 class=' mt-[-5px] text-lg'>OR</h1>
        </div>
    </div>
    
    
    <input type="text" placeholder="Enter your email..." class=" px-[2%] border-solid w-full rounded-lg h-[6%] mt-[5%] border-[#f1f1f1] border-4 ">
    <input type="text" placeholder="Enter your password..." class=" px-[2%] border-solid w-full rounded-lg h-[6%] my-[2%] border-[#f1f1f1] border-4 ">

    <div class=" w-full items-center pt-3 flex justify-between">
        <div class="flex w-[50%] items-center">
            <input type='checkbox' class=' h-6 w-6  focus:ring-0 ' />
            <h1 class="ml-[3%] text-xl font-bold">Remember me</h1>
        </div>
        <p class=" underline text-xl font-semibold">Forgot password?</p>
    </div>

    <div class=" bg-[#242527] w-full h-[6%] text-white text-xl flex justify-center items-center rounded-xl mt-[4%]">Sign in</div>

    <div class="text-black flex text-xl w-full mt-[5%] justify-center">
        <h1>Don't have an account yet?</h1>
        <h1 class='text-white'>d</h1>
        <h1 class='underline font-semibold'>Sign up</h1>
    </div>
    
</div>