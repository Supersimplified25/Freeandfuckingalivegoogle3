<div align="center">
<h1>๐๐๐ง๐ฎ๐๐ฅ๐ฅ๐ฒ ๐๐๐ฉ๐ฅ๐จ๐ฒ ๐๐ฅ๐จ๐ง๐๐๐จ๐ญ ๐ฏ๐ข๐ ๐๐๐ซ๐จ๐ค๐ฎ ๐ ๐๐ข๐ญ๐ก๐ฎ๐ ๐๐๐ญ๐ข๐จ๐ง๐ฌ</h1>
<h3>๐๐ฉ๐ช๐ด ๐ฑ๐ข๐จ๐ฆ ๐ธ๐ช๐ญ๐ญ ๐ต๐ฆ๐ญ๐ญ ๐บ๐ฐ๐ถ ๐ฉ๐ฐ๐ธ ๐ต๐ฐ ๐ฅ๐ฆ๐ฑ๐ญ๐ฐ๐บ ๐๐ญ๐ฐ๐ฏ๐ฆ๐๐ฐ๐ต ๐ต๐ฐ ๐๐ฆ๐ณ๐ฐ๐ฌ๐ถ ๐ธ๐ช๐ต๐ฉ๐ฐ๐ถ๐ต ๐ด๐ถ๐ด๐ฑ๐ฆ๐ฏ๐ด๐ช๐ฐ๐ฏ ๐ถ๐ด๐ช๐ฏ๐จ ๐๐ช๐ต๐ฉ๐ถ๐ฃ ๐๐ค๐ต๐ช๐ฐ๐ฏ๐ด</h3>
</div>

๐ฆ๐๐ก๐-
> ๐๐ผ ๐ป๐ผ๐ ๐๐ฏ๐๐๐ฒ ๐๐ต๐ถ๐ ๐ฆ๐ฒ๐ฟ๐๐ถ๐ฐ๐ฒ ๐ฒ๐น๐๐ฒ ๐๐ถ๐๐ต๐๐ฏ ๐บ๐ถ๐ด๐ต๐ ๐ณ๐น๐ฎ๐ด ๐๐ผ๐๐ฟ ๐๐ฐ๐ฐ๐ผ๐๐ป๐


### ๐Pre Requisites
[Heroku Account](https://heroku.com) --- ๐ฟ๐๐๐ ๐๐๐๐ ๐๐๐๐๐๐๐ ๐๐ ๐๐๐ ๐ฟ๐๐๐๐๐๐๐ ๐๐ ๐๐๐๐๐๐ ๐๐๐ ๐ญ๐๐

[Telegram Account](https://telegram.org) --- ๐ฟ๐๐๐ ๐๐ ๐๐๐ ๐ฟ๐๐๐๐๐๐๐ ๐๐ ๐๐๐ ๐๐๐ ๐ญ๐๐

[TG Bot Token](https://t.me/BotFather) --- ๐ฒ๐๐ ๐๐๐๐ ๐ญ๐๐ ๐ฟ๐๐๐๐ ๐๐ ๐๐๐๐๐ ๐๐๐ ๐ญ๐๐

### Deployment instructions,Some Recomendations and Notes๐ค

๐ท **Here I Don't Provide any Deploy button to heroku, We Use Github Actions to Deploy container to Heroku**
 
๐ท **Make sure to Set the vars correctly in Github-Actions** โDont edit/delete any ENV vars from heroku or Dont add any new vars from heroku either...
   > **to edit/add/del ENV vars...Simply go to github actions and rerun the workflow**

๐ท **If you edit any file or Stuff from Git-Repo you will have to RE-RUN the workflow again or else you will face no changes LOL** 

#### Steps

๐1. **Fork this Repo**

๐2. **Go to Repository `Settings` -> `Secrets`**
    ![Secrets](assets/step-1.png)
    
๐3. **Now set the below Variables in the Github Repository Secrets**
    [Environmental Variables]
	
	> group_ids = your telegram group ID (leave it blank if you don't want to add one). To get your group id, go to @MissRose_bot and type /id
    > 
    > telegram_token = go to @BotFather and send /newbot to get one
	>
    > user_ids = Your user id (go to @MissRose_bot and type /id to get your id) - If you want to authorize multiple users, add a comma between each ID (ex: 150654065,5897065)
	>
	> HEROKU_EMAIL = Just Give the email you used for Heroku Account
	>
	> HEROKU_API_KEY = Get it from ---->(https://dashboard.heroku.com/account/applications/authorizations/new)
	>
	> HEROKU_APP_NAME = Heroku app name that needs to be Updated or Created (Should be in lowercase)
	

๐4. **After filling the Required vars .... go to Actions and then tap on Run the Workflow**
    ![Actions](assets/step-2.png)

๐5. **Now wait it for it to deployed to Heroku and Check app logs and Turn on Workers If OFF** **if everything is OK then send /start to the bot and Bot shall reply.
