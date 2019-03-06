node {

stage('Clone Repository')
{
checkout scm
}


stage('Show me the files')
{
sh "ls -l"
}


stage('Build Docker Image and push image to DockerHub')

{
sh "docker build -t cyn:version1 ."
}
  
stage('Docker login to hub and push the image'){
sh "docker login -u 'cwairoto' -p 'Catalan4810!"
sh "docker tag cyn:version1 cwairoto/cii:latest"
sh "docker push cwairoto/cii:latest"
}


stage('Apply changes to the environment')
{
sh "ls -l"
}




}

