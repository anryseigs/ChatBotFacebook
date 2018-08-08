#Facebook Messenger Bot
This is a simple python template that use Flask to build a webhook for 
Facebook's Messenger Bot API. Original source: https://blog.hartleybrody.com/fb-messenger-bot/

Added information: Install `python, pip, Herolu toolbelt` and from your 
command prompt.
1. virtualenv venv
2. pip install -r requitements.txt (Be required before upload to heroku.)
3. heroku: heroku create (Heroku app is created in heroku.com before you 
upload from local desktop)
4. heroku local
5. git push heroku master
6. heroku open (App must active until step 11.) (If you used git in upper 
folder and created origin and remote, you must open one app only. Please 
remote multiple apps or specify one app if your git config includes many 
heroku apps)
7. Create page "your home page" from facebook.com and create app at developer
.facebook.com
8. app setting: APP_ID, SECRET (copy and paste to heroku app's setting)
9. app product messenger settings: token generator - select page and copy 
PAGE ACCESS TOKEN.
10. Before setup next step, plz make sure
    - [1] "https://xxx.herokuapp.com" works
    - [2] command does`heroku config:add 
    PAGE_ACCESS_TOKEN=$your_page_token_from_step9`
    - [3] check : `heroku config:set FACEBOOK_APP_ID=your_fb_id_from_step8`
    - [4] If so, go to herolu app website and change config value.
11. FB webhook - type verify token with your any string. Type URL callback 
with your heroku app URL.
12. In 10[4], add step11's verify token
13. Subscribe page 
14. Start chatbot (enable messenger from your page. Page is ready to chat now)
15. Other user access to this page and try to chat in messenger button.
16. using TF learning result into bot