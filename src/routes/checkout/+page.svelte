<script>
    import Footer from '../../components/footer.svelte';
    import Logo from '../../lib/assets/creatorvaultlogo.png'

    /** @type {import('./$types').PageData} */
    export let data;
</script>

<main>
    <div class="w-4/5 mx-auto mt-10">
        <div class="grid grid-cols-2">
            <div>
                <img src={Logo} alt="Creator Vault Logo" width="350px" height="3oopx"> 
                <hr class="bg-black h-1 w-3/4 "> 
                <div class="flex flex-col pt-4">
                    <h1 class="text-xl font-bold"> Contact Information</h1>
                    <input class="w-3/4 border border-black rounded-md p-1" type="email" placeholder="e-mail" > 
                </div>
                <div class="flex pt-3 ">
                    <h1 class="text-xl font-bold"> Shipping Information</h1>
                    <div>
                        
                    </div>

                    
                </div>
            </div>
            <div class="bg-slate-100 rounded-lg p-2">
                <h1> Order Information</h1>
            </div>

        </div>
    </div>
    <Footer />
</main>