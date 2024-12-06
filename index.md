
<head>
    <title>Home</title>
    <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1">
</head>
<body>
	
<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			
			console.log("inside");
			window.addEventListener("onEmbeddedMessagingReady", () => {
			console.log("Received the onEmbeddedMessagingReady event…");

			// Send data to Salesforce
			embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({"LoggedInUserFullName" : "Test User ","LoggedInUserLanguage" : "en_US","LoggedInUserEmail" : "test@messaging.com","OrganizationId" : "1020341;15631_MALMO_SRU;GERMANY_EUD_MCSTAGE;"});
			});
			
			embeddedservice_bootstrap.init(
				'00DbY000009Xtwb',
				'IA_Sweden_Service',
				'https://abb--sfdcstage.sandbox.my.site.com/ESWIASwedenService1719400976288',
				{
					scrt2URL: 'https://abb--sfdcstage.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://abb--sfdcstage.sandbox.my.site.com/ESWIASwedenService1719400976288/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

</body>
