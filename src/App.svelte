<script>
    import { onMount } from 'svelte';
    import Navbar from "./Navbar.svelte";

    onMount(() => {
        // Add any necessary JavaScript code here
    });

    let email = '';

    function handleEmailSubmit() {
        // Add logic to handle the email submission here
        console.log('Email submitted:', email);
        // You can clear the email input field here if needed
        email = '';
    }
</script>

<style>
    .bg-gradient {
        position: absolute;
        top: 0;
        right: 0;
        width: 55%;
        height: 100%;
        /*background: linear-gradient(135deg, rgba(66, 153, 225, 0.8), rgba(129, 209, 235, 0.8));*/
        background: linear-gradient(135deg, hsla(272, 82%, 50%, 1) 0%, hsl(255, 98%, 60%) 100%);
        transform: skewX(-20deg);
        translate: 185px;
        box-shadow: inset 0 10px 20px rgba(0, 0, 0, 0.6);
        z-index: -1;
    }

    .text-gradient {
        display: inline-block;
        font-family: helvetica, arial, sans-serif;
        font-weight: bold;
        background: linear-gradient(290deg, WHITE 79.25%, rgb(17 24 39) 20.75%);
        background-clip: text;
        -webkit-text-fill-color: transparent;
        text-rendering: optimizeLegibility;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-shadow: 1px 1px 1px rgba(0,0,0,0.004);
    }

    .button-gradient {
        background: linear-gradient(290deg, #ff4444 90%,  WHITE 10%);
        outline: none;
        -moz-appearance: none;
        -webkit-appearance: none;

    }

    .input-gradient {
        background: linear-gradient(110deg, white 99%, #ff4444 1%);
        outline: none;
        appearance: none;
        -moz-appearance: none;
        -webkit-appearance: none;
    }

    .vignette {
        box-shadow: 0 0 100px rgba(0,0,0,0.9) inset;
    }
</style>

<Navbar></Navbar>

<main class="relative  min-h-screen flex items-center justify-center vignette">
    <div class="bg-gradient"></div>
    <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
            <h1 class="text-4xl font-extrabold text-gray-900 sm:text-5xl md:text-8xl">
                Welcome to <span class="text-gradient">E</span><span class="text-white">ngage</span>
            </h1>
            <p class="mt-3 max-w-md mx-auto text-base text-gray-500 sm:text-lg md:mt-5 md:text-xl md:max-w-3xl">
                The AI-powered personal finance manager that <span class="text-white"> saves you money and time. </span>
            </p>
            <div class="mt-5 max-w-md mx-auto sm:flex sm:justify-center md:mt-8">
                <div class="rounded-md">
                    <form on:submit|preventDefault={handleEmailSubmit}>
                        <div class="flex items-center shadow-2xl">
                            <input type="email" required class="z-10 rounded-l-md input-gradient p-4 text-lg text-gray-900 placeholder-gray-500" placeholder="Enter your email address" bind:value={email} />
                            <button type="submit" class="z-10 button-gradient inline-flex font-bold items-center text-xl px-[40px] py-[16px] rounded-r-md text-white">
                                Notify Me
                            </button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</main>
