I had to try this assignment again because first time I made some error. So i had to use another webserver and network. Please excuse me for this.

1. Opened terminal, changed the path and typed "docker network create webnet".
2. Later I built my image by typing " docker build -t havish-site ."
3. After successfull building, I typed "docker network create network" where I used network instead of webnet.
4. Now I created a simple API container. I typed "docker run -d --name pi --network network hashicorp/http-echo -text="Hello from the API!" " where I changed the names for proper running.
5. Now I updated my Nginx static page to include a button or link that fetches /api from the API container. For that I typed " docker run -d --name net-server --network network -p 7070:80 havish-site".
6. Now the final step. To demonstrate connectivity.. For that I typed "docker exec net-server curl http://api:5678"

This is how I did assignment 2.
The jpeg file is attached.

THANK YOU
