node {   
    echo 'Hello World'   git 'https://github.com/savishy/spring-petclinic'
    properties([buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '2')), pipelineTriggers([pollSCM('H 1 * * *')])])
    bat 'mvn.cmd install'
    archiveArtifacts '**/*.war'
    }
