<html lang="en">
<style type='text/css'>
	.embeddedServiceHelpButton .helpButton .uiButton {
		background-color: #005290;
		font-family: "Arial", sans-serif;
	}
	.embeddedServiceHelpButton .helpButton .uiButton:focus {
		outline: 1px solid #005290;
	}
</style>

<script type='text/javascript' src='https://service.force.com/embeddedservice/5.0/esw.min.js'></script>
<script type='text/javascript'>
	var initESW = function(gslbBaseURL) {
		embedded_svc.settings.displayHelpButton = true; //Or false
		embedded_svc.settings.language = ''; //For example, enter 'en' or 'en-US'

		//embedded_svc.settings.defaultMinimizedText = '...'; //(Defaults to Chat with an Expert)
		//embedded_svc.settings.disabledMinimizedText = '...'; //(Defaults to Agent Offline)

		//embedded_svc.settings.loadingText = ''; //(Defaults to Loading)
		//embedded_svc.settings.storageDomain = 'yourdomain.com'; //(Sets the domain for your deployment so that visitors can navigate subdomains during a chat session)

		// Settings for Field Service

		embedded_svc.settings.enabledFeatures = ['FieldService'];
		embedded_svc.settings.entryFeature = 'FieldService';

		embedded_svc.settings.useCustomAuthentication = false;
		embedded_svc.settings.loginClientId = '';
		embedded_svc.settings.loginRedirectURL = '';
		embedded_svc.settings.loginTargetQuerySelector = '';
		embedded_svc.settings.authenticationStartLabel = '';

		embedded_svc.init(
			'https://haporg--apmdev.sandbox.my.salesforce.com',
			'https://apd.myportal.hap.org/',
			gslbBaseURL,
			'00D6u000000Gyun',
			'Scheduler',
			{
				
			}
		);
	};

	if (!window.embedded_svc) {
		var s = document.createElement('script');
		s.setAttribute('src', 'https://haporg--apmdev.sandbox.my.salesforce.com/embeddedservice/5.0/esw.min.js');
		s.onload = function() {
			initESW(null);
		};
		document.body.appendChild(s);
	} else {
		initESW('https://service.force.com');
	}
</script>
</html>
