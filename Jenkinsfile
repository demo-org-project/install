#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/demo-org-project/install'],
    pipelineTriggers([ upstream(
      threshold: 'SUCCESS',
      upstreamProjects: 'https://github.com/demo-org-project/compile'
    )])])

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
    
    }
}
