===================================================================================================================
29-06-2015

KaizenCommerce v 0.0.2
=

RELEASE NOTE:
=
Minor Fix

CHANGES
=
After issues encountered with the SendGrid Account being used fro phishing emails by malicios intruders details pertainning to external services used by KaizenCommerce have been removed from the CMS. Information such as:

1. Email delivery service SendGrid requires an API Key and Username. These two have been removed from ./application/libraries/Email_Assistant.php. They should be provided before pushing up to production.

2. PayNow payment recieval service requires an Integration ID & Integration KEY. These two have been removed from ./application/controllers/paynow.php. They should be provided before pushing to production.

The exploit discovered came as a result of the code to the CMS living on GitHUb. Although it was under a PRIVATE REPO the code if searched was accessible to the public.

Proof of exploit:
https://github.com/search?q=theTechRebel+sendgrid&ref=searchresults&type=Code&utf8=%E2%9C%93

Fix:
https://sendgrid.com/blog/update-on-security-incident-and-additional-security-measures/



THOUGHTS
=

Hackers are real.


@theTechRebel
=


===================================================================================================================
28-06-2015

KaizenCommerce V 0.0.1
=

RELEASE NOTE: 
=
Initial Commit of KaizenCommerce CMS



CHANGES
=



TO-DOS
=

1. Change ./application/views folder structure to:
			FOLDER_NAME - {representing a module}/ FILE_NAME.php - {represents a particular view file}
			e.g: 
			auth/login.php

2. Get rid of ./client_side/** in favour of using ./uiux/**
			And Front-End folder notation should follow the pattern: FRAMEWORK_NAME/VERSION_USED/FILES.css|.js|min.css|**
			e.g:
			./uiux/bootstrap/3.1.4/
			./uiux/foundation/5/
			./uiux/jquery/1.9.8/

3. Add Plugins Folder in .uiux/plugins/PLUGIN_NAME
			e.g:
			./uiux/plugins/owl-couresel/1.0.3/
			./uiux/plugins/handlebars/1.2.2/

4. Document each controllers function and scope


THOUGHTS
=

In the beginning there was KaizenCommerce. 


@theTechRebel
=
