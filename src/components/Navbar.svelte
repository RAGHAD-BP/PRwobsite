<script>
    import {Button} from "$lib/components/ui/button";
    import ThemeSwitch from "$lib/components/ThemeSwitch.svelte";
    import {page} from "$app/stores";
    const links=[{
        text:'About me',
        href:'./'
        },{
        text:'Project',
        href:'./projects'
    },{
        text: ' Contect ',
        href:'./contact'
    }];
    import * as Sheet from "$lib/components/ui/sheet";
    let isSheetOpen=false;
</script>
<div class="w-[100dvw] bg-secondary text-foreground py-8 px-4  " >
<nav class="max-w-screen-2xl flex justify-between items-center   ">
    <div class="flex items-center gap-2 ">
        <div class="bg-primary h-5 w-5 me-1"/>
        <div>
            <span class="font-bold text-2xl">Raghad Alsuwayhi</span>
            <span class="text-xl">/ Web Developer</span>
        </div>
    </div>
    <div>
    <div class="uppercase hidden md:flex">
            {#each links as link}

                <Button
                        class=" {$page.url.pathname=='link.href'&&' bg-primary'}"
                        href={link.href} variant="link">
                    {link.text}
                </Button>
                {/each}
    </div>

        <Sheet.Root bind:open={isSheetOpen}>
            <Sheet.Trigger class="flex md:hidden">  <Button  variant="ghost" size="icon">
                            <svg xmlns="http://www.w3.org/2000/svg" width="2em" height="2em" viewBox="0 0 16 16">
                                <path fill="none"
                                stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M2.75 12.25h10.5m-10.5-4h10.5m-10.5-4h10.5" />
                           </svg>
                     </Button>  </Sheet.Trigger>
            <Sheet.Content class="flex flex-col items-center justify-center">
                {#each links as link}
                    <Button
                            class="text-xl {$page.url.pathname=='link.href'&&' bg-primary'}"
                            href={link.href} variant="link"
                        on:click={()=>isSheetOpen=false}>
                        {link.text}

                    </Button>
                {/each}
            </Sheet.Content>
        </Sheet.Root>
        <ThemeSwitch/>
    </div>
</nav>
    </div>