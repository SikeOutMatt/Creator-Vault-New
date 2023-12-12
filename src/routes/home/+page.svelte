<script>
    import Header from "../../components/header.svelte";
    import Logo from '../../lib/assets/creatorvaultlogo.png'
    import profilePicture from '../../lib/assets/profilepic.jpeg'
    import bunnyPic from '../../lib/assets/bunnypic.jpeg'
    import Footer from '../../components/footer.svelte'
    import mobileLogo from '../../lib/assets/CreatorVaultMobile.png'
    /** @type {import('./$types').PageData} */
</script>


<main>
    <Header />

    <div class="w-full md:w-3/5  mx-auto"> 
        <div class="justify-center items-center flex">
            <img src={Logo} alt="logo" width="550" height="500">
        </div>
        <div class="flex mx-auto pt-4 w-3/4 md:w-2/4 items-center justify-center">
            <input class="rounded-l-lg h-10 pl-2 w-full border-2 border-[#111111]  " type="search" placeholder="Search for Creators " >
            <button class="bg-black  text-white font-bold p-2 rounded-r-lg "> Search </button>
        </div>
    </div>
    <section class=" mt-4 lg:w-3/5 md:w-4/5 w-full px-3 sm:mx-auto grid lg:grid-cols-5 md:grid-cols-3 grid-cols-2 gap-3"> 
       <a href="/profile"> <div class="bg-[#111111] rounded-t-xl">
            <img class="object-cover rounded-t-xl" src={bunnyPic} alt="profile picture"  >
            <div class="flex justify-center items-center">
                <h1 class="text-xl text-[#f7fbfc] font-bold"> BunnyFuFuu </h1>
            </div>
        </div> </a>
        <a href="/home"> <div class="bg-[#111111] rounded-t-xl">
            <img class="rounded-t-xl" src={profilePicture} alt="profile picture"  >
            <div class="flex justify-center items-center">
                <h1 class="text-xl text-[#f7fbfc] font-bold"> Samantha </h1>
            </div>
        </div> </a>
        <a href="/home"> <div class="bg-[#111111] rounded-t-xl">
            <img class="rounded-t-xl" src={profilePicture} alt="profile picture"  >
            <div class="flex justify-center items-center">
                <h1 class="text-xl text-[#f7fbfc] font-bold"> Jimothy </h1>
            </div>
        </div> </a>
        <a href="/home"> <div class="bg-[#111111] rounded-t-xl">
            <img class="rounded-t-xl" src={profilePicture} alt="profile picture"  >
            <div class="flex justify-center items-center">
                <h1 class="text-xl text-[#f7fbfc] font-bold"> Marty </h1>
            </div>
        </div> </a>
        <a href="/home"> <div class="bg-[#111111] rounded-t-xl">
            <img class="rounded-t-xl" src={profilePicture} alt="profile picture"  >
            <div class="flex justify-center items-center">
                <h1 class="text-xl text-[#f7fbfc] font-bold"> Bella </h1>
            </div>
        </div> </a>
        <a href="/home"> <div class="bg-[#111111] rounded-t-xl">
            <img class="rounded-t-xl" src={profilePicture} alt="profile picture"  >
            <div class="flex justify-center items-center">
                <h1 class="text-xl text-[#f7fbfc] font-bold"> Emily </h1>
            </div>
        </div> </a>
        <a href="/home"> <div class="bg-[#111111] rounded-t-xl">
            <img class="rounded-t-xl" src={profilePicture} alt="profile picture"  >
            <div class="flex justify-center items-center">
                <h1 class="text-xl text-[#f7fbfc] font-bold"> Marie </h1>
            </div>
        </div> </a>

    </section>

    <Footer /> 
</main>