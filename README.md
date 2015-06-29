KaizenCommerce
======

eCommerce CMS Developed by AfriKaizen Inc. 2015 | http://www.afrikaizen.co.zw/
Based on the CodeIgniter framework. | http://www.codeigniter.com/

Environments.
=

Development Environment: 
http://localhost/kaizen/kaizencommerce/



*When pushing up to production change: 

1. ./application/config/config.php : $config['base_url'] to production values 
			e.g: 
			http://localhost/kaizen/kaizencommerce to https://kaizencommerce.co.zw/

2. ./application/controllers/catalogue.php : define('url','localhost/kaizen/kaizencommerce/'); to production values.
			e.g: 
			define('url','localhost/kaizen/kaizencommerce/'); to define('url','https://kaizencommerce.co.zw/');


Getting Started
=

1. Create Database via Phpmydmin named kaizencommerce
2. Import database file ./kaizencommerce.sql into the database you created in step 1
3. in your www folder or htdocs create folders kaizen/kaizencommerce
4. Copy current repo into kaizen/kaizencommerce
5. Email delivery service SendGrid requires an API Key and Username. These two have been removed from ./application/libraries/Email_Assistant.php. They should be provided before pushing up to production.
6. PayNow payment recieval service requires an Integration ID & Integration KEY. These two have been removed from ./application/controllers/paynow.php. They should be provided before pushing to production.


