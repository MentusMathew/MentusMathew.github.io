<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<link rel="stylesheet" href="./custom.css">
<style>
    .slds-visual-picker_vertical .slds-visual-picker__figure {
        height: inherit !important;
    }

    .runtime_appointmentbookingFlowLocation .slds-visual-picker_vertical {
        display: inline-flex !important;
    }
</style>
</head>
<body>
<style type='text/css'>
	.embeddedServiceHelpButton .helpButton .uiButton {
		background-color: #FE6701;
		font-family: "Arial", sans-serif;
                font-size: 15 px;
		font-weight:bold;
		
	}
	.embeddedServiceHelpButton .helpButton .uiButton:focus {
		outline: 1px solid #FE6701;
	}
</style>

<script type='text/javascript' src='https://service.force.com/embeddedservice/5.0/esw.min.js'></script>
<script type='text/javascript'>
	var initESW = function(gslbBaseURL) {
		embedded_svc.settings.displayHelpButton = true; //Or false
		embedded_svc.settings.language = ''; //For example, enter 'en' or 'en-US'

		embedded_svc.settings.defaultMinimizedText = '...'; //(Defaults to Chat with an Expert)
		//embedded_svc.settings.disabledMinimizedText = '...'; //(Defaults to Agent Offline)

		//embedded_svc.settings.loadingText = ''; //(Defaults to Loading)
		//embedded_svc.settings.storageDomain = 'yourdomain.com'; //(Sets the domain for your deployment so that visitors can navigate subdomains during a chat session)

		// Settings for Chat
		//embedded_svc.settings.directToButtonRouting = function(prechatFormData) {
			// Dynamically changes the button ID based on what the visitor enters in the pre-chat form.
			// Returns a valid button ID.
		//};
		//embedded_svc.settings.prepopulatedPrechatFields = {}; //Sets the auto-population of pre-chat form fields
		//embedded_svc.settings.fallbackRouting = []; //An array of button IDs, user IDs, or userId_buttonId
		//embedded_svc.settings.offlineSupportMinimizedText = '...'; //(Defaults to Contact Us)

		embedded_svc.settings.enabledFeatures = ['LiveAgent'];
		embedded_svc.settings.entryFeature = 'LiveAgent';

		embedded_svc.init(
			'https://haporg--pocmmathew.sandbox.my.salesforce.com',
			'https://haporg--pocmmathew.sandbox.my.site.com/producers',
			gslbBaseURL,
			'00D8N000001GiHv',
			'Live_Chat',
			{
				baseLiveAgentContentURL: 'https://c.la2s-core1.sfdc-lywfpd.salesforceliveagent.com/content',
				deploymentId: '5727V0000004D7Q',
				buttonId: '5737V0000004DOe',
				baseLiveAgentURL: 'https://d.la2s-core1.sfdc-lywfpd.salesforceliveagent.com/chat',
				eswLiveAgentDevName: 'Live_Chat',
				isOfflineSupportEnabled: false
			}
		);
	};

	if (!window.embedded_svc) {
		var s = document.createElement('script');
		s.setAttribute('src', 'https://haporg--pocmmathew.sandbox.my.salesforce.com/embeddedservice/5.0/esw.min.js');
		s.onload = function() {
			initESW(null);
		};
		document.body.appendChild(s);
	} else {
		initESW('https://service.force.com');
	}
</script>

</body>
</html>
