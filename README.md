# dockersamples

# commands for webpage
<p> To containerize the Static HTML site. We will create the code and dockerfile and image. Then we will run the container via docker image and push the docker image to Docker Hub Registry</p>
<ul><li>
  mkdir webpage</li><li>
  cd webpage</li><li>
  ls</li><li>
  touch index.html</li><li>
  ls</li><li>
  vi index.html</li><li>
  ls</li><li>
  vi dockerfile</li><li>
  ls</li><li>
  docker build -t web-image:v1 .</li><li>
  ls</li><li>
  docker images</li><li>
  docker run -d -p 80:80 html-server-image:v1</li><li>
  ls -la</li><li>
  docker run -d -p 80:80 web-image:v1</li><li>
  curl localhost:80</li><li>
  docker login</li><li>
  ls</li><li>
  cd webpage/</li><li>
  docker build . -t smulampa/webpage</li><li>
  docker push smulampa/webpage</li></ul>