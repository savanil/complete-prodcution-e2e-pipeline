pipeline{
    agent{
        label "jenkins-agent"
    }
    tools{
        jdk "Java17"
        maven "Maven3"
    }

    stages{
        stage("Clean Workspace"){
            steps{
                cleanWs()
            }
        }

        stage("Checkout from SCM"){
            steps{
                git branch: 'prep', 
                    credentialsId: 'github', 
                    url: 'https://github.com/savanil/complete-prodcution-e2e-pipeline.git'
            }
        }

        // stage("Build Application"){
        //     steps{

        //     }
        // }

        // stage("Test Application"){
        //     steps{

        //     } 
        // }
    }

}