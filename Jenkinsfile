@Library("Shared") _
pipeline{
    agent any
    
    stages{
        stage("Code"){
            steps{
                echo 'cloning the git repo'
                script{
                cloneRepo("https://github.com/shoeb5401/Docker-java-quote.git","main")
            }
                echo 'Cloned Successfully'
    }    }
//     stage('Check Docker Info') {
//     steps {
//         sh 'docker info'
//     }
// }
        stage("Build"){
            steps{
            echo "Building the image"
            script{
            docker_build("java-app","v2","shoeb5401")
            }
            echo "Image Build Successfull!!!"
            }
        }
        stage("Run"){
            steps{
            echo "Deploying the image on the machine!!!"
           
        }}
    }
       
}
