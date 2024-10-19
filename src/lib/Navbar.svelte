<script lang="ts">
    export let links = [
        { name: "About Me", href: "#about-me" },
        { name: "My Projects", href: "#projects" },
        { name: "Experience", href: "#experience" },
    ];
</script>

<nav class="fixed top-0 left-0 w-full text-white shadow-md z-50 navbar">
    <div class="flex w-full justify-between p-6">
        <div class="font-bold text-xl">
            <a aria-current="page" class="" href="/"
                ><div
                    data-aos="fade-in"
                    data-aos-delay="500"
                    class="Logo-module--wrapper--Uu4re aos-init aos-animate"
                >
                    <img src="" alt="Irina Bubela" />
                </div>
            </a>
        </div>
        <div class="space-x-6">
            {#each links as link}
                <a href={link.href} class="hover:text-gray-300">{link.name}</a>
            {/each}
        </div>
    </div>
</nav>

<style lang="scss">
    .navbar {
        align-items: center;
        background-color: transparent;
        background-color: #0a0616;
        border-bottom: 1px solid #1a1820;
        display: flex;
        height: 80px;
        left: 0;
        padding: 0 40px;
        position: fixed;
        right: 0;
        top: 0;
        z-index: 3;
    }
    
    a {
        color: #fff;
        font-size: 0.7rem;
        font-weight: 600;
        padding: 8px 0;
        text-decoration: none;
        text-transform: uppercase;
        transition: all 0.2s ease;
    }
</style>
