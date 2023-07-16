pipeline {
    agent any
    options {
        skipDefaultCheckout(true)
    }

    stages {

        stage('Checkout SCM') {
            steps {
                script {
                    checkout scm
                }
                
            }
        }

        
        stage('Run PowerShell Script') {
            steps {
                script {
                    Status = powershell(returnStatus: true, script: ".\\HelloWorld.ps1")
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