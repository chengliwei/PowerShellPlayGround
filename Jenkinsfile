pipeline {
    agent any
    
    environment {
            PATH = "C:\\WINDOWS\\SYSTEM32"
        }
    stages {
        stage('CLean Workspace') {
            steps {
                cleanWs()
            }
        }
        stage('Run PowerShell Script') {
            steps {
                bat 'powershell.exe -File HelloWorld.ps1'
            }
        }
    }
}