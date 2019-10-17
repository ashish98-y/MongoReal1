pipelines {
    stages{
        stage("checkout"){
            steps{
                git 'https://github.com/ashish98-y/MongoReal1.git'
            }
        }
        stage("deploy"){
            steps{
                sh label: '', script: 'ansible-playbook -i dev.inventory mongodb.yml'
            }
        }
    }
}
