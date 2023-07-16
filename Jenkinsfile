pipeline {
    agent any

    stages {

        
        stage('Run PowerShell Script') {
            steps {
                script {
                    Status = Powershell(returnStatus: true, script: ".\\HelloWorld.ps1")
                }
                
            }
        }

        stage('Clean Workspace') {
            steps {
                cleanWs()
            }
        }
    }
}