<script>
	import { t } from "svelte-i18n";
	import LanguageRadio from "./components/language-radio.svelte";
</script>

<style global lang="scss">
	@import './app.scss';
</style>

<main>
	<h1>{$t('title')}</h1>
	<p>{$t('msg1')}<a href="https://svelte.dev/tutorial">{$t('msg2')}</a>{$t('msg3')}</p>
	<div class="options">
		<LanguageRadio iso='en' />
		<LanguageRadio iso='pt' class="radio" />
	</div>
</main>
