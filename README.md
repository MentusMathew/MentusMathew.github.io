<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<link rel="stylesheet" href="./custom.css">
</head>
<body>
<div id="lexcontainer">
</div>
<div class="row"><div class="component plain-html col-12">
    <div class="component-content">
<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00Ddl000001XOKj',
				'Live_Chat_Embedded_Deployment',
				'https://haporg--devmerge.sandbox.my.site.com/ESWLiveChatEmbeddedDep1738126593973',
				{
					scrt2URL: 'https://haporg--devmerge.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://haporg--devmerge.sandbox.my.site.com/ESWLiveChatEmbeddedDep1738126593973/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'>
</script>
</div></div>
        </div>
</body>
</html>
