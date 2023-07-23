pipeline{
    agent{ lable 'JDK-17'}
    triggers { pollSCM('* * * * *')}
stages{
    stage('git'){
        steps{
            git branch: 'master',
                url: 'https://github.com/jenkinsci/jenkins.git'              
        }
    }    
    stage('build'){
        steps{
            sh 'ls'
            sh 'pwd'
            sh 'maven package' 
        }
    }    
    }
}

    
