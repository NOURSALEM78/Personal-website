<script>
import Container from "$lib/components/Container.svelte";
import Title from "$lib/components/title.svelte";
import Input  from "$lib/components/ui/input/input.svelte";
import Label  from "$lib/components/ui/label/label.svelte";
import Textarea from "$lib/components/ui/textarea/textarea.svelte";
import Button from "$lib/components/ui/button/button.svelte"
</script>
<title>
    Contact
</title>

<Container class="flex flex-col gap-12">
    <Title title="تواصل معي"/>
    <form 
        action="https://formsubmit.co/noursalm261@gmail.com" method="POST"
        class="bg-secondary p-4 flex flex-col gap-6 ">
            <Label for="name">إسمك </Label>
            <Input required name="naame" id="name" placeholder="اكتب/ي اسمك"/>

            <Label for="name"> إيميلك </Label>
            <Input required type="email" name="naame" id="name" 
            placeholder="youruser@email.com"/>

            <Label for="supject"> الموضوع </Label>
            <Input required name="supject" id="supject" placeholder="عنوان الرساله"/>

            <Label for="massage"> الرساله </Label>
            <Textarea required name="massage" id="massage" placeholder=" رسالتك"/>
            <Button type="submit">
                إرسال
            </Button>
    </form>
</Container>