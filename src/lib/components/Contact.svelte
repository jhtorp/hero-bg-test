<script>
	import { send } from 'emailjs-com';

	async function handleSubmit(event) {
		event.preventDefault();
		const botField = event.target.elements['bot-field'];
		if (botField.value !== '') {
			return;
		}
		const message = {
			name: event.target.elements['name'].value,
			email: event.target.elements['email'].value,
			message: event.target.elements['message'].value
		};
		try {
			await send('service_n2uloko', 'template_xmmo16z', message, 'SuMszKb6Tev7wsMD8');
			alert('Your message was sent successfully!');
		} catch (error) {
			alert('There was an error sending your message. Please try again later.');
			console.error(error);
		}
	}
</script>

<form on:submit|preventDefault={handleSubmit}>
	<label for="name">Name:</label>
	<input type="text" id="name" name="name" required />
	<label for="email">Email:</label>
	<input type="email" id="email" name="email" required />
	<label for="message">Message:</label>
	<textarea id="message" name="message" required />
	<input type="text" name="bot-field" style="display:none" />
	<button type="submit">Submit</button>
</form>

<style>
	form {
		display: flex;
		flex-direction: column;
		gap: 10px;
	}
</style>
