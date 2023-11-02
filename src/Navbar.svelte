<script>
    import { onMount } from 'svelte';

    onMount(() => {
        // Add any necessary JavaScript code here
    });
</script>

<style>
    .navbar {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        background-color: #ffffff;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        z-index: 999;
    }

    .navbar .logo {
        font-size: 1.5rem;
        font-weight: bold;
        color: #333333;
    }

    .navbar .nav-links {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .navbar .nav-links a {
        margin-left: 1.5rem;
        color: #666666;
        text-decoration: none;
        transition: color 0.3s ease;
    }

    .navbar .nav-links a:hover {
        color: #333333;
    }

    .content {
        margin-top: 4rem; /* Adjust this value to create space below the navbar */
    }
</style>

<header class="navbar">
    <div class="max-w-3xl mx-auto px-4 sm:px-6 lg:px-8">
        <nav class="flex items-center justify-between h-16">
            <div class="logo">
                Engage
            </div>
            <div class="nav-links">
                <a href="#">Home</a>
                <a href="#">Features</a>
                <a href="#">Pricing</a>
                <a href="#">Contact</a>
            </div>
        </nav>
    </div>
</header>