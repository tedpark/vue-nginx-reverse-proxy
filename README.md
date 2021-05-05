# Bundle multiple Vue application into a single domain name via nginx reverse proxy

key point to serve frontend application on a different location are as the following:

- first: each route should have prefix url (gateway: nginx.conf line 24)
- second: application nginx should serve the base path (forntend-dashboard: nginx.conf line 25-28)
- third: static files should serve under "/dashboard" directory (forntend-dashboard: Dockerfile line 10)

### Useful links

- Frontend / path: [http://localhost](http://localhost)
- Frontend /dashboard path: [http://localhost/dashboard](http://localhost/dashboard)
- Backend /api path: [http://localhost/api](http://localhost/api)
