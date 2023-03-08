 
pipeline {
    agent any
    parameters {
        choice(name: 'VERSION', choices: ['1.1.0', '1.2.0', '1.3.0'], description: '')
        booleanParam(name: 'executeTests', defaultValue: true, description: '')
    }
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
             steps {
                script {
            git url: 'https://github.com/testorgarchit/codeqldemo.git'
        }  
                 }
            }
        stage('Download CodeQL CLI Bundle') {
            steps {
               // sh "wget https://github.com/github/codeql-action/releases/latest/download/codeql-bundle-win64.tar.gz -O ..\codeql-bundle-win64.tar.gz"
                //sh "tar xzvf ..\codeql-bundle-win64.tar.gz -C ..\"
                //sh "del ..\codeql-bundle-win64.tar.gz"
                //sh "cd ..\; set PATH=%cd%\codeql;%PATH%"
            }
        }

    }   
}
