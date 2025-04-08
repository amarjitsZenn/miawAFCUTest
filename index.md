<html>
  <body>
    <script type='text/javascript'>
		function initEmbeddedMessaging() {
			try {
				window.addEventListener("onEmbeddedMessagingReady", () => {
					console.log("Received the onEmbeddedMessagingReady event…");
				
					// Send data to Salesforce
					embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({"userName" : "123456789",
						"memberName" : "John"});
				});

				embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

				embeddedservice_bootstrap.init(
					'00D8c000006ft3Q',
					'afcuGitHubMIAWTest',
					'https://zenndatahubfsc-dev-ed.my.site.com/ESWafcuGitHubMIAWTest1744075904134',
					{
						scrt2URL: 'https://zenndatahubfsc-dev-ed.my.salesforce-scrt.com'
					}
				);
			} catch (err) {
				console.error('Error loading Embedded Messaging: ', err);
			}
		};
	</script>

	<script type='text/javascript' src='https://zenndatahubfsc-dev-ed.my.site.com/ESWafcuGitHubMIAWTest1744075904134/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

  </body>
</html>
