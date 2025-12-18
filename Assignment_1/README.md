1.I have created a simple html file named index. It has the page name as my name and remaining details.
2.I have created a docker file through VS code.
3.I saved both the files in a folder named dock.

4.Later i have changed the path to the folder so that docker can access my files.
5.After that i have put the code "docker build -t havish-site ."  in order to build the image.
6.Later i have used "docker run -d --name my-running-assignment -p 7070:80 havish-site" inorder to run the container so it’s accessible on port 7070 on the host.
7.Next, I opened my browser and typed "http://localhost:7070" to see if the container was working. Also i typed "curl http://localhost:7070" in the terminal. This gave me a html code of my page print out in the terminal.
8.Later stopped my assignment using "docker stop my-running-assignment" and removed the container by typing "docker rm my-running-assignment"

This is how i did assignment 1.

