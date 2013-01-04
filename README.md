#MDN Sample

This is only a composer package test. Don't take it serious. 

##Install

###Setting Up Your VHOST

The following is a sample VHOST you might want to consider for your project.

    <VirtualHost *:80>
       DocumentRoot "/whatever"
       ServerName local.mdn-sample

       # This should be omitted in the production environment
       SetEnv APPLICATION_ENV development

       <Directory "/whatever">
           Options Indexes MultiViews FollowSymLinks
           AllowOverride All
           Order allow,deny
           Allow from all
       </Directory>

    </VirtualHost>