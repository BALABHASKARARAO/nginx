pipeline {
    agent any
    stages {
        stage('DeployToEkS-cluster') {
            steps {
                kubernetesDeploy(
                    kubeconfigId: 'kubernetes-kubeconfig',
                    configs: 'nginx.yaml',
                    enableConfigSubstitution: true
                )
            }
        }
    }
}
