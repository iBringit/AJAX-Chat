To prevent errors like

ChatBot: Error: Connection status: 403

To prevent this error on Nginx Server not reverse proxy.

Lets say you have the chatroom in a subfolder of your project directory called chat.. 

In Nginx conf for the site you want the chat enabled, add this

location /chat/ {
    index index.php;
    autoindex on;
}

ChatBot: Error: Connection status: 403 will go away.
