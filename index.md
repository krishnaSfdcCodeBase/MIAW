<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00D1x000000Ja3A',
				'PA_NORTHERN_HUB',
				'https://abb--comint.sandbox.my.site.com/ESWPANORTHERNHUB1716987000569',
				{
					scrt2URL: 'https://abb--comint.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://abb--comint.sandbox.my.site.com/ESWPANORTHERNHUB1716987000569/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
