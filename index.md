<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			window.addEventListener("onEmbeddedMessagingReady", () => {
			console.log("Received the onEmbeddedMessagingReady event…");

			// Send data to Salesforce
			embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({"LoggedInUserFirstName" : "Test ","LoggedInUserLastName" : "krishna","LoggedInUserEmail" : "test@messaging.com"});
			});
			embeddedservice_bootstrap.init(
				'00D9M000000qSBX',
				'IA_Northern_US_HUB_Service',
				'https://abb--comstage.sandbox.my.site.com/ESWPANorthernHub1708684533261',
				{
					scrt2URL: 'https://abb--comstage.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://abb--comstage.sandbox.my.site.com/ESWPANorthernHub1708684533261/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
