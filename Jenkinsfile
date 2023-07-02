pipeline {
    agent any

    stages {
        stage('CLean Workspace') {
            steps {
                cleanWs()
            }
        }

        environment {
            PATH = "C:\\WINDOWS\\SYSTEM32"
        }
        stage('Run PowerShell Script') {
            steps {
                bat 'powershell.exe -File HelloWorld.ps1'
            }
        }
    }
}