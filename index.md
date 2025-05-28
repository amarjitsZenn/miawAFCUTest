<html>
  <body>
	 <script type='text/javascript'>
		function initEmbeddedMessaging() {
			try {
				embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
	
				embeddedservice_bootstrap.init(
					'00DOy00000FuqeQ',
					'Live_Agent_Chat_Test_Deployment',
					'https://1source--devzencbqa.sandbox.my.site.com/ESWLiveAgentChatTestD1748447068703',
					{
						scrt2URL: 'https://1source--devzencbqa.sandbox.my.salesforce-scrt.com'
					}
				);
			} catch (err) {
				console.error('Error loading Embedded Messaging: ', err);
			}
		};
	</script>
	<script type='text/javascript' src='https://1source--devzencbqa.sandbox.my.site.com/ESWLiveAgentChatTestD1748447068703/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
  </body>
</html>
