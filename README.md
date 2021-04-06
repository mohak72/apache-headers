# apache-headers
#Content-Security

Header add Content-Security-Policy "default-src *  data: blob: filesystem: about: ws: wss: 'unsafe-inline' 'unsafe-eval' 'unsafe-dynamic'; script-src * data: blob: 'unsafe-inline' 'unsafe-eval'; connect-src * data: blob: 'unsafe-inline'; img-src * data: blob: 'unsafe-inline'; frame-src * data: blob: ; style-src * data: blob: 'unsafe-inline'; font-src * data: blob: 'unsafe-inline';"
#Referrer-Policy
Header set Referrer-Policy "same-origin"
#Permissions-Policy
Header always set Permissions-Policy "geolocation=(),midi=(),sync-xhr=(),microphone=(),camera=(),magnetometer=(),gyroscope=(),fullscreen=(self),payment=()"
#X-Content-Type
<IfModule mod_headers.c>
Header set X-Content-Type-Options "nosniff"
</IfModule>


