# Web APP

- App Service Plan is responsible for building the compute infrastructure which is responsible for runnign th web applications.
- Evry WebvApp must be part of an App Service Plan
- An ASP can contain multiple Web Apps.
- Free ASP (F1) has 60 minutes CPU/day
- Shared ASP (D1) has 240 CPU minutes/day
- ASP has following plans-
  - Free, Shared, Basic, Standard, Premium and Isolated
  - From Basic plan onwards, we can create multile instances as per the plan to handle multple Apps and CPU load
- If you want to add another web app under same ASP then you have to choose the same region which ASP has otherwise you wont be able to choose that ASP for other regions.
- If the ASP was created /built for Windows then App containing the runtime stack/code other than Windows like lInux etc then that ASP plan can be chosen. Only those runtiem stack/language can be chosen for whcih the ASP OS was created.
- Map Custom Domain with web app
  - Go to App Service WebApp and go to Custom Domain Menu
  - Give the custom domain name and click on validate via CNAME or via A record
  - To validate, first verify ownership of domain by adding TXT or CNAME record with DNS provider
  - Add the CNAME record in DNS provider
  - Click on Validate again to verify Domain Ownership
  - Now click on Add custom domain to add onc validation is succeeded
- Adding SSL
  - Go to TLS/SSL settings and check for certificates
  - Create App Service Managemd Certificates
  - Go to Bindings and Bind your custom domain with certificate thumbprint
- App Service Logs
  - Logs either on FileSystems, Blobs.
  - Logs of Application, Web Server.
- Log Stream gives real time logs of Application logs and Web Server Logs

  
