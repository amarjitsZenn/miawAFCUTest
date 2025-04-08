<!DOCTYPE html>
<html>
<head>
  <title>Bot Test Page</title>
</head>
<body>
  <h1>Testing Embedded Salesforce Chatbot</h1>

  <!-- Your Embed Script Here -->
  <script type='text/javascript'>
    function initEmbeddedMessaging() {
      try {
        embeddedservice_bootstrap.settings.language = 'en_US';

        embeddedservice_bootstrap.init(
          '00D8c000006ft3Q',
          'afcuTester',
          'https://zenndatahubfsc-dev-ed.my.site.com/ESWafcuTester1744070346552',
          {
            scrt2URL: 'https://zenndatahubfsc-dev-ed.my.salesforce-scrt.com'
          }
        );
      } catch (err) {
        console.error('Error loading Embedded Messaging: ', err);
      }
    };
  </script>
  <script type='text/javascript' src='https://zenndatahubfsc-dev-ed.my.site.com/ESWafcuTester1744070346552/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

</body>
</html>
