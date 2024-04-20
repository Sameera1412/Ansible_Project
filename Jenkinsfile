pipeline{
  agent any
  stages{
    stage{
      step ("Executing nginx playbook") {
        ansiblePlaybook become: true, credentialsId: 'Jenkins_Ansible', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'inventory', playbook: 'nginx.yml', vaultTmpPath: ''
      }
    }
  }
}
