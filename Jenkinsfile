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
sh "docker tag cyn:version1 cwairoto/cii:version1"
sh "docker push cwairoto/cii:version1"
}


stage('Apply changes to the environment')
{
sh "ls -l"
}




}

