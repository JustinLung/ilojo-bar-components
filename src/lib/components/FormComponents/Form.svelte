<script lang="ts">
	import FormContainer from './FormContainer.svelte';
	import Title from './Title.svelte';
	import Label from './Label.svelte';
	import Input from './Input.svelte';
	import Button from './Button.svelte';
	import Textarea from './Textarea.svelte';
	import Image from './Image.svelte';
</script>

<FormContainer>
	<Title />
	<Label labelName="name" labelText="Name" />
	<Input inputName="name" placeholder="John Doe" />
	<Label labelName="email" labelText="Your email" />
	<Input inputName="email" placeholder="johndoe@mail.com" />
	<Label labelName="storytitle" labelText="Storytitle" />
	<Input inputName="storytitle" placeholder="Awesome story!" />
	<Label labelName="content" labelText="Content" />
	<Textarea placeholder="Lorem ipsum" />
	<Button btnText="Send Story" />
</FormContainer>
