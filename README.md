The Discord bot that we are going to build will listen for the keyword $meme and responds with a random meme from Reddit.

We'll be creating and registering our Discord Application inside the Developer Portal. Then, we will create a Bot for the application and get the required permissions.

Step 1. Go to Developer Portal
Visit https://discord.com/developers/applications and sign in if you haven't already.

Step 2. Create a New Application
To let Discord know we're going to be connecting to their backend servers, we need to register an application and set up the required permissions.

Click "New Application" on the top right.

Next, give your application a name. Here, we are calling ours MemeBot:

Step 3. Add a Bot to Your Application
Find the "Bot" tab in the left panel:

And click "Add Bot":

Step 4. Get the Token for Your Application
This step is important because we'll need this Token for later. This Token is similar to a password for your application. Anybody who has this can control it. (So make sure to never share your bot token with anyone, or upload it on GitHub by mistake!)

Click "Reset Token", write it down somewhere safe and definitely don't put it in any public place.

Lastly, while we're still on the "Bot" tab, scroll down until you find a section about "Privileged Gateway Intents." In order for our Discord bot to receive messages, we'll need to toggle the "Message Content Intent" under this section:

Turning this on in the developer portal will allow us to properly set up our bot in the code later in this project.

Step 5. Invite Application to Your Server
Now that we've set up our first application, we have to create an invite, to get our bot into our Discord server. To do that we can click URL Generator and select the following permissions. In the screenshot below, we are telling Discord to create an invitation link for our application with the scope "Bot" and that bot should be able to "Send Messages." (Note: Be careful with granting the all-powerful "Administrator" permission to your bot).


This is the link to invite our application (Discord bot) into a Discord server. Copy and paste this link into another tab in your browser and invite the bot into the Discord server that you want.

You can confirm if this worked by checking for this message in your Discord server.

Alright, now that we’ve set up our coding environment and got the necessary permissions from Discord for our new application, let’s write some code.
