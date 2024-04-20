pipeline 
{
  agent any
  stages 
  {
    stage ("Executing nginx playbook") 
    {
      steps
      {
        ansiblePlaybook become: true, credentialsId: 'Ansible_client_credentials', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'inventory', playbook: 'nginx.yml', vaultTmpPath: ''
      }
    }
  }
}
