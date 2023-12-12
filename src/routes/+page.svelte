<script>
import Header from "../components/header.svelte";
import Banner from '../lib/assets/Frontpagebanner.webp';
import Logo from '../lib/assets/LogoWhite.png'




    
</script>



<main class="bg-slate-900 m-0 min-w-screen min-h-screen">
    <div class=" flex flex-col  lg:grid grid-cols-2">
        <div>
            <img class=" lg:max-h-screen max-h-52" src={Banner} alt="banner" width="100%">
        </div>
        <div class="flex flex-col justify-center align-middle">
            <img src={Logo} alt="logo" width="500" height="500" class="mx-auto mb-4">
            <a class="mx-auto w-8/12 bg-sky-400 rounded-md text-white font-bold py-1 text-sm my-2 text-center " href="/home"> <button> Login </button></a> 
            <a></a><button class="bg-sky-400 rounded-md w-8/12 mx-auto text-white font-bold py-1 text-sm my-2"> Sign Up </button>
            <hr class="h-1 my-8 bg-white border-0 dark:bg-gray-700">
            <h4 class="mx-auto text-white font-medium my-2"> Sign In with your favorite Apps</h4>
            <button class="bg-sky-400 rounded-md w-8/12 mx-auto text-white font-bold py-1 text-sm my-2"> Sign in with Google </button>
            <button class="bg-sky-400 rounded-md w-8/12 mx-auto text-white font-bold py-1 text-sm my-2"> Sign in with X </button>
            <button class="bg-sky-400 rounded-md w-8/12 mx-auto text-white font-bold py-1 text-sm mt-2 mb-5"> Sign in with Facebook </button>
           </div>
    </div>


</main>


