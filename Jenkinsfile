#!/usr/bin/env groovy

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
				bat 'LabVIEWCLI.exe -OperationName ExecuteBuildSpec -ProjectPath %WORKSPACE%\\CITestBed.lvproj -TargetName "My Computer" -BuildSpecName My_Application'
				}
        }
        stage('Test') {
            steps {
                echo 'Testing...'
				bat 'LabVIEWCLI.exe -OperationName RunVI -VIPath %WORKSPACE%\\TestMain.vi main.vi
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
