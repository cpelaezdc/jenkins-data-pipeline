pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'whoami'
                    // Install pip if maybe not installed in current machine
                    // -y to automatic Yes to prompts
                    sh 'sudo apt install -y python3-pip'
                    // Choisissez la commande en fonction de votre script
                    sh 'sudo pip install pandas' // Installer les dépendances
                    sh 'python3 data_analysis.py' // Exécuter le script Python
                    sh 'ls'
                }
            }
        }
    }
}