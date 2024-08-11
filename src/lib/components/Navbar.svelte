<script>
import {Button} from "$lib/components/ui/button";
</script>

<nav class="flex justify-between w-[100dvw] bg-secondary text-secondary-foreground py-8 px-4 ">
    <div class="flex items-center gap-2 text-2xl">
        <div class="bg-primary h-5 w-5 me-1"/>
        <span class="font-bold">Raghad Alsuwayhi</span>
        <span>/ Web Developer</span>
    </div>
<div>
    <Button href="./" variant="link">
        About me
    </Button>
    <Button href="./resume" variant="link">
    Resume
    </Button>
    <Button href="./projects"variant="link">
        Project
    </Button>
    <Button href="./contact" variant="link">
        Contect
    </Button>
</div>
</nav>