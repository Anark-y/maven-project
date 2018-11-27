import hudson.tasks.test.AbstractTestResultAction
import hudson.model.Actionable
import hudson.tasks.junit.CaseResult

node 
{
    echo "Stage 1. EverythingBeforeDeploy"
    git credentialsId: 'c0e5e9ee-4eb3-ac87-8a4e-bfcd91a6567b', url: 'https://github.com/Anark-y/maven-project'


    echo "Stage 2. This job mocks a Chapoo_Master/MvnSite_Pipeline job. After this we will re-use the workspace"

    echo "Stage 3 Stashing all the things"
    archiveArtifacts artifacts: '**/*.war'
}     
  
