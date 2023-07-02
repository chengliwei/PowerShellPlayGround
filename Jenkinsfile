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
                Status = powershell(label:POWERSHELL: Description", returnStatus: true, script: "HelloWorld.ps1")
            }
        }
    }
}