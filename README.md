# Wordpress  

# BEGIN WordPress  
<IfModule mod_rewrite.c>  
RewriteEngine On  
RewriteCond %{HTTP_HOST} ^mydictionaryplus.com$ [OR]  
RewriteCond %{HTTP_HOST} ^www.mydictionaryplus.com$  
RewriteRule (.*)$ http://tudien.tructuyen247.com/$1 [R=301,L]  
</IfModule>  

Chuyen huong toan bo domain  
