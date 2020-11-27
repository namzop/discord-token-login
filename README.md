<h1 align = "center"> Discord Token Login </h1>

### THIS METHOD DOESN'T WORK ON PHONE

Okay, So Many Youtubers fool you by making you download an app to login with discord token but there is an easy way in which you don't have to download any app. 

<strong>It will work on the website as well as the discord client. </strong>

Now, you need to logout from the account if you have already logged in with some other one. Now when you get the login screen like this - 
<img src = "https://github.com/namzop/discord-token-login/blob/main/assets/image_2020-11-27_18-44-11.png?raw=true">

Now you have to press <code> CTRL+SHIFT+I
</code> Now you will see this kind of thing - 
<img src = "https://github.com/namzop/discord-token-login/blob/main/assets/inspect%20element%20pic.jpg?raw=true">
Now you have to click on the ```console``` , if you can't see it then just check the image I have underlined it with yellow!!

After clicking on it, the console with show something like this - 
<img src = "https://github.com/namzop/discord-token-login/blob/main/assets/console%20img.jpg?raw=true">

Now you have to paste this exactly as it's given - 
```
function login(token) {
setInterval(() => {
document.body.appendChild(document.createElement `iframe`).contentWindow.localStorage.token = `"${token}"`
}, 50);
setTimeout(() => {
location.reload();
}, 2500);
}```
```
And Press Enter

If you don't paste it correctly, then the console will give an error. 
After pasting this, if it replies with ```undefined``` then you are going the right way!!

Now the <strong> final </strong> step. 
You know just have to paste this -
<code> login("your-token-here") </code>
in the place of token, you have to paste your <i> (or the token of the account you want to login to) </i> 

<strong> Congrats!! Now you're logged in </strong> 

It will log you out as soon as you will close or reload the discord client or page. 

### Contributors 

<img src = "https://github.com/namzop/discord-token-login/blob/main/assets/contributors%201.jpg?raw=true"> 

[Namz](https://namz.gq)





