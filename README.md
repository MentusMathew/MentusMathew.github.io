<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<link rel="stylesheet" href="./custom.css">
</head>
<body>
  <h1>TEST</h1>
  <style type='text/css'>
	.embeddedServiceHelpButton .helpButton .uiButton {
		background-color: #0081A1;
		font-family: "Chivo", sans-serif;
	}
	.embeddedServiceHelpButton .helpButton .uiButton:focus {
		outline: 1px solid #0081A1;
	}

        .slds-icon-utility-minimize-window{
    		zoom: 120%;
	 }       
    	 .slds-icon-utility-close{
          	zoom: 120%;
     	  }
    
    	 .slds-form-element__label{
        	font-size:1.5ch;
       	}
</style>
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
</body>
</html>
