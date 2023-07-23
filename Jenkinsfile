pipeline{
    agent{ lable 'JDK-17'}
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
            sh 'maven package' 
        }
    }    
    }
}

    
