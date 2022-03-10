pipeline{
    agent any
    stages{
        stage("git clone"){
            steps{
                git 'git@github.com:myproject2022/myapp-ansible.git'
            }
        }
        stage("execute ansible"){
            steps{
               ansiblePlaybook  installation: 'ansible211', inventory: 'dev.inv', playbook: 'apache.yml'
            }
        }
    }
}
