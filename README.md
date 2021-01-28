# apache-reverse-proxy-nginx


            root   /var/www/html
            proxy_pass http://127.0.0.1:8080/;
            proxy_redirect off;
            proxy_set_header Host $http_host;
            proxy_set_header X-Real-IP $remote_addr;
            
            
proxy_redirect off; 
proxy_set_header Host $host; 
proxy_set_header X-Real-IP $remote_addr; 
proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; 
proxy_max_temp_file_size 0; 
client_max_body_size 10m; 
client_body_buffer_size 128k; 
proxy_connect_timeout 90; 
proxy_send_timeout 90; 
proxy_read_timeout 90; 
proxy_buffer_size 4k; 
proxy_buffers 4 32k; 
proxy_busy_buffers_size 64k; 
proxy_temp_file_write_size 64k; 
      
<?php
  phpinfo();
?>
