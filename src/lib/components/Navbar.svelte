<script>
    import {Button} from "$lib/components/ui/button";
    import ThemeSwitch from "$lib/components/ThemeSwitch.svelte";
    import {page} from "$app/stores";
</script>
<div class="w-[100dvw] bg-secondary text-foreground py-8 px-4  " >
<nav class="max-w-screen-2xl flex justify-between items-baseline   ">
    <div class="flex items-center gap-2 ">
        <div class="bg-primary h-5 w-5 me-1"/>
        <div>
            <span class="font-bold text-2xl">Raghad Alsuwayhi</span>
            <span class="text-xl">/ Web Developer</span>
        </div>
    </div>
    <div class="uppercase">
        <Button
                class=" {$page.url.pathname=='/'&&' bg-primary'}"
                href="./" variant="link">
            About me
        </Button>
        <Button
                class=" {$page.url.pathname=='/resume'&&' bg-primary'}"
                href="./resume" variant="link">
            Resume
        </Button>
        <Button
                class=" {$page.url.pathname=='/projects'&&' bg-primary'}"
                href="./projects"variant="link">
            Project
        </Button>
        <Button
                class=" {$page.url.pathname=='/contact'&&' bg-primary'}"
                href="./contact" variant="link">
            Contect
        </Button>
        <ThemeSwitch/>
    </div>
</nav>
</div>