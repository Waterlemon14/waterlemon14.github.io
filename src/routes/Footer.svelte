<script>
    import Icon from '@iconify/svelte';

    import {
        GitHub, 
        LinkedIn,
        Email,
        Profile
    } from '$lib/assets'

    import {
        gitHubURL,
        linkedInURL,
        portfolioGitHubURL
    } from '$lib/info'

</script>

<footer class="bg-blue-950 p-4 text-gray-400 sm:p-6">
    <div class="mx-auto max-w-screen-xl">
        <div class="md:flex md:justify-between">
            <div class="mb-6 md:mb-0">
                <a href="/portfolio" class="flex items-center">
                    <img src={Profile} alt="Dancing Duck" width="500" height="500" loading="lazy" class="mr-3 size-8" />
                    <span class="self-center whitespace-nowrap text-2xl font-semibold text-white">Eisenhower Aldemita II</span>
                </a>
            </div>
            <div class="grid grid-cols-3 gap-8 sm:gap-6">
                <div>
                    <h2 class="mb-4 text-sm font-semibold uppercase text-white">Sitemap</h2>
                    <ul class="space-y-2 text-gray-400">
                        <li><a href="/portfolio" class="hover:underline">Home</a></li>
                        <li><a href="/portfolio/projects/" class="hover:underline">Projects</a></li>
                        <li><a href="/portfolio/research/" class="hover:underline">Research</a></li>
                    </ul>
                </div>
                <div>
                    <h2 class="mb-4 text-sm font-semibold uppercase text-white">Social</h2>
                    <ul class="space-y-2 text-gray-400">
                        <li>
                            <a href={linkedInURL} target="_blank" class="hover:underline"
                                >LinkedIn</a
                            >
                        </li>
                        <li>
                            <a href={gitHubURL} target="_blank" class="hover:underline"
                                >GitHub</a
                            >
                        </li>
                    </ul>
                </div>
                <div>
                    <h2 class="mb-4 text-sm font-semibold uppercase text-white">Code</h2>
                    <ul class="space-y-2 text-gray-400">
                        <li>
                            <!-- to update link to portfolio repo -->
                            <a href={portfolioGitHubURL} target="_blank" class="hover:underline"
                                >Portfolio Repo</a
                            >
                        </li>
                        <!-- <li>
                            <a href={githubURL} target="_blank" class="hover:underline"
                                >External Assets</a
                            >
                        </li> -->
                    </ul>
                </div>
            </div>
        </div>
        <hr class="my-6 border-gray-700 sm:mx-auto lg:my-8" />
        <div class="sm:flex sm:items-center sm:justify-between">
            <span class="text-sm text-gray-400 sm:text-center"
                >&copy; 2025 <a href="/portfolio" class="hover:underline">Eisenhower Aldemita II</a>. All rights reserved.
            </span>
            <div class="mt-4 flex space-x-6 sm:mt-0 sm:justify-center">
                <a href="mailto:edaldemita@up.edu.ph" title="edaldemita@up.edu.ph" target="_blank"
                    ><Icon icon={Email} width="20" height="20" /></a
                >
                <a href={linkedInURL} title="LinkedIn" target="_blank"
                    ><Icon icon={LinkedIn} width="20" height="20" /></a
                >
                <a href={gitHubURL} title="GitHub" target="_blank"
                    ><Icon icon={GitHub} width="20" height="20" /></a
                >
            </div>
        </div>
    </div>
</footer>