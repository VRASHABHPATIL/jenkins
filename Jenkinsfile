pipeline{
    agent {label 'agent1'}
    stages{
        stage("git-clone"){
            steps{
                echo "cloning from rfepository"
                git url:"https://github.com/VRASHABHPATIL/jenkins.git",branch:"main"
                echo "cloning completed"
            }
        }
        stage("deployment"){
            steps{
                echo "building the image started and deployment also started "
                sh "docker-compose up -d "
                echo "building and deployment completed"
            }
        }
    }
}
