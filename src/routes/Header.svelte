<script>
    import { Profile } from '$lib/assets';
</script>

<header class="sticky top-0 z-10 w-full bg-blue-200 shadow-md">
    <nav class="grid grid-cols-2">
        <div class="flex justify-start">
            <a class="block px-4 py-2 transition-colors hover:bg-hover" href="/portfolio">
                <img
                    src={Profile}
                    width="500"
                    height="500"
                    alt="dancing duck"
                    class="block size-10 rounded-full shadow-xl"
                />
            </a>
        </div>
        <ul class="flex justify-end">
            <li>
                <a class="block p-4 hover:underline" href="/portfolio/projects">Projects</a>
            </li>
            <li>
            </li>
            <li>
                <a class="block p-4 hover:underline" href="/portfolio/research">Research</a>
            </li>
        </ul>
    </nav>
</header>