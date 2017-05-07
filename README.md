# FacebookPageAutomation
A python script to post content to facebook page using Graph API. Set up a cronjob to run every x minutes as per your businees need.

Engaging customers and/or fans on social media is essential to remain on top of the game. As such, you have to publish post(content) constantly. On your own(time) or hire(money) a right person to do so. You have no other options. Or do you ? I created a quick script to publish post on one of my facebook page and assigned a cronjob to run it every 5 minutes. That's 288 posts(content) per day. 8640 per month. Do the math for yourself. 

# Flow
1. Looks for an excel file with content to publish. 
2. If file not found, scrapes content from planetpython.org and adds to excel file in the format(content title, content url)
3. Checks for a text file which stores the count of the rows in the sheet that has been published. If file not found starts from second row. 
4. Publishes the content at row number x from step 3 
5. Increases the count in the text file. 
