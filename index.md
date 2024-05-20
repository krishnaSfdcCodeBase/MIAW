<html>
  <body>
      <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00D7E000000AlHh',
				'PA_Northern_HUB',
				'https://abb--comsupport.sandbox.my.site.com/ESWPANorthernHUB1706678888610',
				{
					scrt2URL: 'https://abb--comsupport.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://abb--comsupport.sandbox.my.site.com/ESWPANorthernHUB1706678888610/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

  </body>   
</html>


