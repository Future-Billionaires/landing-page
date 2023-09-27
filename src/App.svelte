<script>
    import { onMount } from 'svelte';

    onMount(() => {
        // Add your custom logic here
    });
</script>

<style>
    /* Add your custom styles here */
    .glass {
        background: rgba(255, 255, 255, 0.5);
        backdrop-filter: blur(10px);
    }
</style>

<main class="bg-gradient-to-b from-purple-500 to-blue-500 min-h-screen">
    <header class="bg-transparent py-4">
        <div class="container mx-auto px-4 flex justify-between items-center">
            <h1 class="text-white text-4xl font-bold">Engage</h1>
            <nav>
                <ul class="flex space-x-10">
                    <li><a href="#" class="text-white hover:text-blue-200">Home</a></li>
                    <li><a href="#" class="text-white hover:text-blue-200">Features</a></li>
                    <li><a href="#" class="text-white hover:text-blue-200">Pricing</a></li>
                    <li><a href="#" class="text-white hover:text-blue-200">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section class="py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="">
                    <h1 class="text-7xl font-bold mb-4 text-white">Revolutionize your finances</h1>
                    <p class="text-xl text-gray-200 mb-4">Engage leverages cutting-edge AI technology to provide personalized financial insights and recommendations.</p>
                </div>
                <div>
                    <img src="assets/financial-illustration.jpg" alt="Financial Illustration" class="w-full h-auto">
                </div>
            </div>
        </div>
    </section>

    <section class="bg-gray-100 py-12">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold mb-8 text-gray-800">Powerful Features</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="glass p-8 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <h3 class="text-2xl font-bold mb-4 text-gray-800">Real-time spending analysis</h3>
                    <p class="text-gray-600 mb-4">Track your expenses in real-time and gain valuable insights into your spending habits.</p>
                </div>
                <div class="glass p-8 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <h3 class="text-2xl font-bold mb-4 text-gray-800">Smart budgeting and savings goals</h3>
                    <p class="text-gray-600 mb-4">Set personalized budgets and savings goals to achieve your financial objectives.</p>
                </div>
                <div class="glass p-8 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <h3 class="text-2xl font-bold mb-4 text-gray-800">Investment portfolio optimization</h3>
                    <p class="text-gray-600 mb-4">Optimize your investment portfolio based on AI-driven recommendations and market trends.</p>
                </div>
            </div>
        </div>
    </section>

    <section class="bg-gray-100 py-12">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-gray-800 text-center mb-8">Our Mission</h2>
            <div class="flex items-center justify-center">
                <div class="w-3/4">
                    <div class="flex flex-col md:flex-row items-center md:items-start justify-center md:justify-between bg-white p-8 rounded-lg shadow-lg">
                        <div class="md:w-1/2 mb-4 md:mb-0">
                            <p class="text-lg text-gray-800">At Engage, we are on a mission to revolutionize the way people manage their finances. We believe that everyone deserves access to intelligent financial solutions that simplify and enhance their financial lives.</p>
                        </div>
                        <div class="md:w-1/2">
                            <p class="text-lg text-gray-800">Through cutting-edge AI technology, we empower individuals and businesses to make informed financial decisions, achieve their goals, and secure their financial future.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>




    <section class="bg-transparent py-12">
        <div class="container mx-auto px-4">
            <h2 class="text-white text-3xl font-bold mb-4 flex items-center justify-center">Join the financial revolution today</h2>
            <p class="text-white mb-4 flex justify-center">Sign up now and experience the power of AI-driven financial management.</p>
            <div class="flex justify-center items-center text-center ">
                <a href="#" class="bg-white text-blue-500 hover:bg-blue-100 py-3 px-6 rounded-full font-bold">Get Started</a>
            </div>
        </div>
    </section>

    <footer class="bg-transparent py-4">
        <div class="container mx-auto px-4">
            <p class="text-white text-center">© 2023 Engage. All rights reserved.</p>
        </div>
    </footer>
</main>
