# Web-Whatsapp-Stalker
An insidious script made to stalk people over WhatsApp based on their online and offline times.

Yes, IKR this is creepy but here goes the story.
I was studying to check how can I track DOM changes in a page and stumbled across JavaScript MutationObserver API.
Whenever someone comes online, the DOM of the contact information in web whatsapp adds a DIV element to display online.
This div tag is removed whenever someone goes offline.

How does it works?

[WEB WHATSAPP OVER BROWSER {Injected JavaScript in Browser Console}] <<<============<<< PROXY(REMOVES CSP RESPONSE HEADER) <<<=============<<<[WHATSAPP SERVER]
          |↓|
          |↓|
          |↓|
          |↓|
          |↓|
          [↓]
   [Local Python Server] >>>>>>>>>>> [Writes Timestamps to .txt File]
   
##################################### HOW TO RUN ##############################################
Follow below steps sequentially

1. Run the python stalkerserver.py.
2. Open web whatsapp and on brup proxy disable the Content-Security-Policy response header.
3. Click on a chat of the target contact person.
4. Open browser JS console and copy paste the stalkerclient.js, hit enter.
5. File 'stalker.txt' will be created on online/offline activity by the target person.
###############################################################################################


Important Note: I assume no responsibilty for misuse :D
What you do can be constructive or distructive and it is your choice and is not on ME!! XD
