node {

       
     
    stage('Clone repository') {        
        /* Cloning the Repository to our Workspace */
        node ('master') {
            checkout scm
        }        
    }

    stage('execute ansible playbook') {
        /* This builds the actual image */
        node ('master') {
            sh 'ansible-playbook main.yml'
        }        
    }
        
   

}
