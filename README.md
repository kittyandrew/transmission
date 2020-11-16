#### Installation / Configuration
Since BasicAuth is set up via Caddy instead of internal Transmission service, don't forget to allow all hosts. To do that open `.config/settings.json` and check following value:  
```
...
"rpc-host-whitelist-enabled": false,
...
```
If it's `true` change the value, to allow connect via local interfaces.  
  
Finally fill `.env` config.  
**Note:** Ensure you have torrent service storage path configured correctly (default in both services)  

#### Deploy
```
docker-compose up -d  
```  

