# RestServer
Basic Server plugin which can be embeded inside your cordova/ionic app.

After you make a request, the request is sent to the index.html file and from there a generical "Hello World!" message is sent by the server
as a response.
So you can edit this response as you want, depending on the services you want to provide, just edit the index.html file on function onRequest()
and use the sendResponse() function to send the response you want.

There is also a serveFile() function on the backend in file named NanoHTTPD.java which is not being used because it was wanted that the request
goes to the index.html file, so if you want to serve html pages, put them on htdocs folder and use the URL:
'(your IP):8080/files/(the path of the page you wanna serve)'.

To use the plugin:

-> create new cordova project: cordova create (put here package name you want)
-> cordova plugin add https://github.com/daniel-ist/RestServer.git
-> cordova platform add android (not tested in IOS)

Then adapt the index.html file the way you want to create your REST webservices.
