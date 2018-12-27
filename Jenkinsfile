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
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
