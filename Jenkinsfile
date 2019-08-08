pipeline{
agent any
stages{
stage('compile')
{
steps{
bat 'mvn compile'
}
}
stage('report')
{ 
steps{
cucumber failedFeaturesNumber: -1, failedScenariosNumber: -1, failedStepsNumber: -1, fileIncludePattern: '**/*.json', pendingStepsNumber: -1, skippedStepsNumber: -1, sortingMethod: 'ALPHABETICAL', undefinedStepsNumber: -1
}
}
}
}
