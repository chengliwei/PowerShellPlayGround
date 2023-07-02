pipeline {
    agent any

    stages {
        stage('CLean Workspace') {
            steps {
                cleanWs()
            }
        stage('Run PowerShell Script') {
            steps {
                bat 'powershell.exe -File HelloWorld.ps1'
            }
        }
    }
}