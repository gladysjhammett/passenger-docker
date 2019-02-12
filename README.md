Why use passenger-docker?
Why use passenger-docker instead of doing everything yourself in Dockerfile?

Your Dockerfile can be smaller.
It reduces the time needed to write a correct Dockerfile. You won't have to worry about the base system and the stack, you can focus on just your app.
It sets up the base system correctly. It's very easy to get the base system wrong, but this image does everything correctly. Learn more.
It drastically reduces the time needed to run docker build, allowing you to iterate your Dockerfile more quickly.
It reduces download time during redeploys. Docker only needs to download the base image once: during the first deploy. On every subsequent deploys, only the changes you make on top of the base image are downloaded.
