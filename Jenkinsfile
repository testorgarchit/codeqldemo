 
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
         
        
         stage('Clone Repository') {
             steps {  
                script { git url: 'https://github.com/testorgarchit/codeqldemo.git'
           
        }  
                 }
            }
     stage("wget") {
            steps {
                script {
                   sh "C:/Users/archi/wget 'https://dl.google.com/android/repository/sdk-tools-linux-4333796.zip'"
                }
            }
        }
          stage('Download CodeQL CLI Bundle') {
            steps {
               script { 
                 sh "wget https://github.com/github/codeql-action/releases/latest/download/codeql-bundle-win64.tar.gz "
                //sh "tar xzvf ..\codeql-bundle-win64.tar.gz -C ..\"
                //sh "del ..\codeql-bundle-win64.tar.gz"
                //sh "cd ..\; set PATH=%cd%\codeql;%PATH%"
               }
               }
        }

    }   
}
