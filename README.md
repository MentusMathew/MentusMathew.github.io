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
<div id="lexcontainer">
</div>
<script src="https://haporg--devmerge.sandbox.my.site.com/scheduleappointment/lightning/lightning.out.js"></script>  
<script>
    var Str1 = window.location.href;    
  // document.write(Str1 + "</br>" );
    var inputVariables = [
         { name : "inputVariables", type : "String", value: Str1 } 

       ];
$Lightning.use("runtime_appointmentbooking:lightningOutGuest",
    function() {                  // Callback once framework and app load
        $Lightning.createComponent(
            "lightning:flow",    // top-level component of your app
            { },    // attributes to set on the component when created
            "lexcontainer",    // the DOM location to insert the component
            function(component) {            // API name of the Flow
                component.startFlow("Inbound_New_Guest_Appointment_Custom",inputVariables); 
            }
        );
    },    'https://haporg--devmerge.sandbox.my.site.com/scheduleappointment/'  
);
</script>
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
