 
pipeline {
    agent any
     
    stages {
        stage("init") {
            steps {
                script {
                   echo "init"
                }
            }
        }
        stage("build") {
            steps {
                script {
                    echo "build"
                    //gv.buildApp()
                }
            }
        }
         
        stage("deploy") {
            steps {
                script {
                    echo "deploy"
                }
            }
        }
         stage('Clone Repository') {
             steps { git url: 'https://github.com/testorgarchit/codeqldemo.git'
                script { git url: 'https://github.com/testorgarchit/codeqldemo.git'
           
        }  
                 }
            }
        

    }   
}
