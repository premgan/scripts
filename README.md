# scripts
Scripts for simplifying troubleshooting, reproductions, etc. 

As we use Fiddler more and more now with newer Apps, here is cool thing I worked on while working on an issue to reduce the repro time from 8 days to 6 minutes. Basically I changed the expiry time to accomplish this. However issue being client all I needed was the client to think the expiry is 6 minutes without making any changes to the service/server. In this case server didn’t even allow lower than 8 hours expiry. 

Basically Fiddler offers a way to create custom rules to modify requests and responses. In this case I modified the response. The key learning here is that these scripts has same syntax as Microsoft.Jscript. This enables us to modufy reequests and responses to debug, throubleshoot, expedite repro(s) etc. 

You can FiddlerChangeExpiry script I wrote to modify the expiry times.So if there are client issues for which you need to wait till expiry you can write similar script for your Apps as well. 
