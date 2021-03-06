# chat_app_using_socket.io_alongwith_cloud_deployment

Live Demo:http://ec2-13-127-221-29.ap-south-1.compute.amazonaws.com/signUpPage

The chatApp is based on MVC structure.Users whoe are new to MVC can read about it here.
https://www.sitepoint.com/node-js-mvc-application/

## Functionalites on which it has been built -

* Node.js     
* express.js   - as a framework 
* mongoDB      - database for saving all type of messages and user personal information
* Jade         - as server side rendering template
* Socket.io    - for Websockets and real time communication
* AWS EC2 Instance
* nginx as a server 

Note :In order to use this webApp on your localhost,simpy download the repository and perform
the following commands in the terminal(make sure the path is set to whehre this repository has been downloaded )
```
npm install --save
node index.js
```
This will run the app on [localhost:3000](http:localhost:3000/signUpPage)


## Steps to use this one to one chatApp built primarily on socket.io.

## Step1

First thing first,you need to signup in order to use the chap by visiting http://ec2-13-127-221-29.ap-south-1.compute.amazonaws.com/signUpPage.

Those who have signed up can go and login at this link http://ec2-13-127-221-29.ap-south-1.compute.amazonaws.com/loginPage

## Step2 

Once the user successfully signUp/login,he will be redirected to choose an option "single chat" or "previous chats" line this.
If their is a new user then obiviously there will be no previous chats for him and he can go ahead and choose single chat option.

### Screenshot1
![screen shot 2018-03-14 at 12 15 23 pm](https://user-images.githubusercontent.com/16476315/37387216-92c3c376-2781-11e8-8ade-2a378e525966.png)

Once single chat option is chosen,he will be redirected to ask a "room name" where he can fill any random string like "mathsGroup","trialRoom" etc but do rememeber the room name.
Once you fill up the room ,you are good to go and you will land up in the chatRoom creeated by you.Now as you would like to chat with someone ,you can just provide him the "room name".
The other user will follow the same steps as mentioned from the starting of step2 and enter the roomaname provided by you.

if all things go well you will land up as per the screenshot below-

### Screenshot2
![screen shot 2018-03-14 at 12 29 05 pm](https://user-images.githubusercontent.com/16476315/37387680-6880ce54-2783-11e8-8d1c-a8cb61516908.png)

if there is an existing user who wants to chat with someone whom he has already talked,he can found out by choosing previous chats option as given in "screenshot1".Once "previous chats" option is choosen ,he will be shown a "friends list" of mentioning the username of all the ones with whom he had talked earlier like this -

### Screenshot3
![screen shot 2018-03-14 at 12 38 39 pm](https://user-images.githubusercontent.com/16476315/37387994-b135df30-2784-11e8-956a-f0d3d6af479c.png)

He( let's say User A) can choose any(let's say User B) of them and he will land up in chatRoom. now if at the same time UserB also likes to chat with User A he can go ahead and choose User A name from his "friends list".As both are online at the same time,they will be land up in same room(this is because of the configuration made by me in the script).

Soon again they both can use the functionalities mentioned below-

1. Both user will be notified about logging In/logging Out 
2. If one is typing another will get notfication that he is typing.
3. User can share images(upto 3-5 mb) and videos (3 -5 mb)too.
4. User can even share thier location.(this fetaure can be used on localhost and if yu want to use it on other online servers ,please make your site secured(https).

![screen shot 2018-03-14 at 3 41 51 pm](https://user-images.githubusercontent.com/16476315/37396272-6e5d9774-279e-11e8-876b-74e184fff704.png)




