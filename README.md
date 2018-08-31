# Wordpress  

# BEGIN WordPress 

<IfModule mod_rewrite.c>   
RewriteEngine On   
RewriteCond %{HTTP_HOST} ^mydictionaryplus.com$ [OR]   
RewriteCond %{HTTP_HOST} ^www.mydictionaryplus.com$   
RewriteRule (.*)$ http://tudien.tructuyen247.com/$1 [R=301,L]   
</IfModule>   

Chuyen huong toan bo domain  


function tomjn_only_upload_for_admin( $file ) {
    if ( ! current_user_can( 'manage_options' ) ) {
        $file['error'] = 'You can\'t upload images without admin privileges!';
    }
    return $file;
}
add_filter( 'wp_handle_upload_prefilter', 'tomjn_only_upload_for_admin' );
