# docker-hello-nodejs

Three file

index.js we specify code for our rest API 
expose at the root line -5 '/' 
and return the response for line -6 back Hello world javascript v1
at line 8 : running at port 5000


package.json
here we are speficiying the dependencies that we would want to have
line 11- express this is framework which we are using to run our rest API & version 4.17.1
to run the application we need to download these dependencies and then able to run application up




So if you look at the Docker file, we'll specify the instructions for it.
So what we are doing is the base image which is being used is Node.
which is being used is Node.
So we are using node and 8.16.1 version of Node.
And as usual, we are using an Alpine image
as the same thing as Python,and we are establishing a working directory,
what we are doing is copy the current directory as slash app
and after that we are doing an NPM install.
If you are new to JavaScript, then NPM is a dependency management tool.
So over here in the package.json,
we specified the dependencies that this application needs
and NPM install would download all those for you.
This is similar to PIP or Maven or
Griddle,
whichever one you are familiar with.
And after that we are exposing
5,000.
And then we are just executing node index.js.
So we are launching the index.js, which is present in here,
using node is.
As you can see, it's a very, very, very simple Docker file
and let's try and build the image for it right now.
Let's see the present working directory.






docker build -t dockerid/nodejs:0.3.3.RELEASE .
