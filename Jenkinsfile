#!/usr/bin/env groovy

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
				bat 'echo %PATH%'
				bat 'LabVIEWCLI.exe -OperationName ExecuteBuildSpec -ProjectPath C:\Users\OpalRTDev\.jenkins\workspace\C:\Users\OpalRTDev\.jenkins\workspace\JenkinsExample_master\CITestBed.lvproj -TargetName "My Computer" -BuildSpecName My_Application'
				}
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
