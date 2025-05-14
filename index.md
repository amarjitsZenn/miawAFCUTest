<html>
  <body>
    <script type='text/javascript'>
		function initEmbeddedMessaging() {
			try {
				window.addEventListener("onEmbeddedMessagingReady", () => {
					console.log("Received the onEmbeddedMessagingReady event…");
				
					// Send data to Salesforce
					embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({
						"memberID" : "123456789",   // Optional, replace with actual member ID.
						"memberFirstName" : "John", // Optional, replace with actual first name.
						"memberLastName" : "Doe",   // Optional, replace with actual last name.
						"messagingChannel": "affinity-mobile-banking", // Required, replace with actual channel name. affinity-mobile-banking, affinity-web, or affinity-banking-web
					});
				});

				embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

				embeddedservice_bootstrap.init(
					'00DOy00000FuqeQ',
					'Test_Bot_Github',
					'https://1source--devzencbqa.sandbox.my.site.com/ESWTestBotGithub1747159519141',
					{
						scrt2URL: 'https://1source--devzencbqa.sandbox.my.salesforce-scrt.com'
					}
				);
			} catch (err) {
				console.error('Error loading Embedded Messaging: ', err);
			}
		};
	</script>

	<script type='text/javascript' src='https://1source--devzencbqa.sandbox.my.site.com/ESWTestBotGithub1747159519141/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

  </body>
</html>
