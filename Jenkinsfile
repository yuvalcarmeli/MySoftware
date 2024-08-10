properties([pipelineTriggers([cron('H/30 * * * *')])])
pipeline{
    agent any

    stages{
        stage('checkout'){
            steps{
                git branch: 'master' , url: "https://github.com/yuvalcarmeli/MySoftware.git"
            }
        }

        stage('Run python'){
            steps{
                sh 'python3 NewScreen.py'
            }
        }
    }
}
