pipeline {
    agent any
    parameters{
        string(name: 'tomcat-dev', defaultValue: '1.2.3.4', description: 'tomcat development server')
        string(name: 'tomcat-prod', defaultValue: '1.2.3.4', description: 'tomcat prod server')
    }
    stages {   
        stage ('Stage Setup'){
            steps{
                echo 'Script Startup'
            }
        }
        stage('Prepare Pipeline') {
            steps {
                sh 'bash ./cd/pipeline-prepare.sh'
            }
        }
    }
}