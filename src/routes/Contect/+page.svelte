<script lang="ts">
    import { Input } from "$lib/components/ui/input/index.js";
    import { Label } from "$lib/components/ui/label/index.js";
    import {Textarea} from "$lib/components/ui/textarea/index.js";
    import {Button} from "$lib/components/ui/button";
</script>
<div class="text-3xl font-bold text-center pt-32 py-10  ">Let's Talk!</div>
<form class="m-14 p-8 bg-secondary "
action="https://formsubmit.co/raghad11ali88@gmail.com"
method="POST">
    <div class="grid w-full items-center gap-3">
        <div>
        <Label for="name">Name</Label>
        <Input required  name="name" id="name" placeholder="write your name" />
        </div><div>
        <Label for="email">Email</Label>
        <Input required type="email" name="email" id="email" placeholder="example1@gmail.com"/></div>
        <div>
            <Label for="subject">Subject</Label>
            <Input required name="subject" id="subject" placeholder="....."/></div>
    <div>
        <Label for="message">Message</Label>
        <Textarea required name="message" id="message" placeholder="write your message" />
            </div>
        <Button type="submit">Send</Button>
</form>