<script>
    import {Button} from "$lib/components/ui/button";
    import ThemeSwitch from "$lib/components/ThemeSwitch.svelte";
</script>
<nav class="flex justify-between items-baseline w-[100dvw] bg-secondary text-secondary-foreground py-8 px-4 ">
    <div class="flex items-center gap-2 ">
        <div class="bg-primary h-5 w-5 me-1"/>
        <div>
<span class="font-bold text-2xl">Raghad Alsuwayhi</span>
<span class="text-xl">/ Web Developer</span>
</div>
</div>
<!--<div class="uppercase">-->
<!--    <Button href="./" variant="link">-->
<!--        About me-->
<!--    </Button>-->
<!--    <Button href="./Project" variant="link">-->
<!--        Project-->
<!--    </Button>-->
<!--    <Button href="./Contect" variant="link">-->
<!--        Contect-->
<!--    </Button>-->

<!--</div>-->
    <ThemeSwitch/>
</nav>