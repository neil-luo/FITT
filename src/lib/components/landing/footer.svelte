<script lang="ts">
    const content = [
        { name: 'About FITT (What)', href: '/about' },
        { name: 'Why do we need FITT (Why)', href: '/why' },
        { name: 'How FITT helps us (How)', href: '/how' },
        { name: 'When FITT helps (When)', href: '/when' },
        { name: 'How to use FITT (How-to)', href: '/how-to' },
    ];
</script>

<footer class="border-t border-border bg-background/95 backdrop-blur supports-[backdrop-filter]:bg-background/60">
    <div class="mx-auto max-w-7xl px-6 pb-8 pt-16 sm:pt-24 lg:px-8 lg:pt-32">
        <div class="xl:grid xl:grid-cols-3 xl:gap-8">
            <!-- Brand section -->
            <div class="space-y-8">
                <div class="flex items-center space-x-2">
                    <span class="text-2xl font-bold text-foreground">FITT ICT task</span>
                </div>
            </div>

            <!-- Navigation sections -->
            <div class="mt-16 grid grid-cols-2 gap-8 xl:col-span-2 xl:mt-0">
                <div class="md:grid md:grid-cols-2 md:gap-8">
                    <div>
                        <h3 class="text-sm font-semibold text-foreground">Content</h3>
                        <ul role="list" class="mt-6 space-y-4">
                            {#each content as item}
                                <li>
                                    <a
                                        href={item.href}
                                        class="text-sm text-muted-foreground hover:text-foreground transition-colors"
                                    >
                                        {item.name}
                                    </a>
                                </li>
                            {/each}
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</footer>
