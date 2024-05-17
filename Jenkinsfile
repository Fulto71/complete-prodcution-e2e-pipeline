pipeline{
 agent{
         label "jenk"
     }
    tools {
        jdk 'Java17'
        maven 'Maven3'
    }
    stages{
        stage("Cleanup Workspace"){
            steps {
                cleanWs()
            }

        }
    
        stage("Checkout from SCM"){
            steps {
             git branch: 'main', timeout: 60, url: 'https://github.com/Fulto71/complete-prodcution-e2e-pipeline'
            }

        }

    }


}
