# PulseRoot
## Secure, fast, and reliable web chat application.

![](https://cdn.discordapp.com/attachments/512111631006957578/513434725160058880/unknown.png)

PulseRoot is a chat application that focuses on reliability, speed, and most of all... **security**.  
It allows you to enter the global chat as either a guest, or gives you the ability to make an account.

With an account, you can:
* Private message other users
* Have your own profile
* Integrate with other services (Twitter, Discord, Google, etc.)

### Running your own PulseRoot
Running your own version of PulseRoot is fairly easy.
That being said, there are steps you will have to take:

#### Cloning and Installing
Clone the repo: `git clone https://www.github.com/SmartieCodes/pulseroot`
In the directory with `package.json`, run `npm install`.

#### Setting up files and variables
* Rename `config.json_example` to `config.json`
* Rename `example.sqlite` to `db.sqlite`
* Change the values in `config.json` to Discord Webhook URLs... or don't. It's optional, after all.
* Go to your Environment Variables configuration.
* Add a value for `SESSION_SECRET`. This is used for Express sessions.

#### Running
In the root directory, run `npm start`.
In addition, you can use `localtunnel` to host your own server: `lt --port 8080`
Congrats, you're now running your own version of PulseRoot!

### Socket.io
PulseRoot utilizes socket.io for messaging.
Read more about socket.io [here](https://socket.io).
