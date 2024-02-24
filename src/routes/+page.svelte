<script>
    import '../app.css'
    import Button from '../components/Button.svelte';
    import {browser} from '$app/environment';

    export let page
    if (browser) {
        page = document.documentElement
    }
    export const switcher = () => {
        if (!page.classList.contains('dark')) {
            page.classList.add('dark')
        }
        else if (page.classList.contains('dark')) {
            page.classList.remove('dark')
        }
    }
    </script>

<div class=" flex flex-col h-[85vh] w-[80vw] lg:w-[50vw] sm:w-[65vw] bg-white dark:bg-[#3b3b3b] rounded-xl shadow-xl columns-1 items-center px-[10%] ">
    <div class="theme-switcher"></div>
    <img class=' h-[7vh] w-[7vh] mt-[2vh] ' src="https://img.icons8.com/ios/50/verified-account.png" alt="verified-account"/> <br />
    <h1 class=" flex justify-center dark:text-white font-bold w-[45vw] xl:w-[20vw] text-xl ">Welcome back</h1>
    <h2 class=" mt-[1vh] dark:text-white text-xl flex text-center ">Please enter your details to sign in</h2>
    <div class=" w-full h-[20%] flex justify-between">
        <Button logo='apple' />
        <Button logo='google' />
        <Button logo='microsoft' />
    </div>
    
    <div class="bg-[#ebebeb] dark:bg-black w-full hidden h-1 md:flex justify-center ">
        <div class=" mt-[-2%] w-[10%] bg-white dark:bg-[#3b3b3b]  justify-center lg:flex hidden">
            <h1 class=' mt-[-0.2vw] dark:text-white text-2xl '>OR</h1>
        </div>
    </div>
    
    
    <input type="text" placeholder="Enter your email..." class=" px-[2%] border-solid w-full rounded-lg dark:bg-black h-[6%] mt-[5%] border-[#f1f1f1] dark:border-gray-500 border-4 ">
    <input type="text" placeholder="Enter your password..." class=" px-[2%] border-solid w-full  rounded-lg h-[6%] dark:bg-black my-[2%] border-[#f1f1f1] border-4 dark:border-gray-500">

    <div class=" w-full items-center pt-3 flex justify-between">
        <div class="flex w-[50%] items-center">
            <input type='checkbox' class=' md:h-6 md:w-6 w-6 h-4 cursor-pointer focus:ring-0 ' />
            <h1 class="ml-[3%] text-sm md:text-xl font-bold dark:text-white">Remember me</h1>
        </div>
        <p class=" underline text-sm md:text-xl  md:ml-[5vh] font-semibold dark:text-white cursor-pointer hover:text-[#000000c4]">Forgot password?</p>
    </div>

    <button on:click={switcher} class=" bg-[#242527] w-full h-[6%] text-white text-xl flex hover:bg-[#000000c4] justify-center items-center rounded-xl my-[4vh]">Sign in</button>

    <div class="text-black flex text-xl w-full mt-[5%] justify-center">
        <h1 class="dark:text-white">Don't have an account yet?</h1><br>
        <h1 class='text-white dark:text-[#3b3b3b]'>d</h1>
        <h1 class='underline font-semibold dark:text-white cursor-pointer hover:text-[#000000c4]'>Sign up</h1>
    </div>
    
</div>