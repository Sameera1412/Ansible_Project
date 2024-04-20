pipeline 
{
  agent any
  stages 
  {
    stage 
    {
      steps ("Executing nginx playbook") 
      {
        ansiblePlaybook become: true, credentialsId: 'Ansible_client_credentials', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'inventory', playbook: 'nginx.yml', vaultTmpPath: ''
      }
    }
  }
}
