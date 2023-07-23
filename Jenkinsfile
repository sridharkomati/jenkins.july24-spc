pipeline{
    agent { label 'JDK-17'}
    tools {
        maven 'maven 3.9.3'
        jdk   'JDK-17'
    }
       
    triggers { pollSCM('* * * * *')}
stages{
    stage('git'){
        steps{
            git branch: 'declarative',
                url: 'https://github.com/sridharkomati/jenkins.july24-spc.git'              
        }
    }    
    stage('build'){
        steps{
            sh 'ls'
            sh 'pwd'
            sh 'mvn --version'
            sh 'mvn package' 
        }
    }    
    }
}

    
