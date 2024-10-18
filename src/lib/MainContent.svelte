<script>
</script>

<section
    class="flex flex-col justify-center items-center h-screen text-center bg-gradient-animated"
>
    <h1 class="text-5xl font-bold mb-4">Hi, my name is Irina.</h1>
    <p class="text-2xl text-gray-700 mb-8">
        Frontend Developer with experience in various JS frameworks and some
        cool personal projects.
    </p>
    <button
 class="bg-white-600 py-3 px-6 rounded-md hover:bg-white-500 transition"
    >
        Contact Me
    </button>
</section>

<style>
    @keyframes gradient {
        0% {
            background-position: 0% 50%;
        }
        50% {
            background-position: 100% 50%;
        }
        100% {
            background-position: 0% 50%;
        }
    }

    .bg-gradient-animated {
        background: linear-gradient(270deg, #4a90e2, #9013fe, #f5a623);
        background-size: 300% 300%;
        animation: gradient 15s ease infinite;
    }
</style>
