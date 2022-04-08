pipeline
{
    node {
    stage('Git pull') 
    {
        git 'https://github.com/ashumesh/s3-bucket.git'
    }
    stage('Deploy')
    {
        sh 'aws s3 ls'
        sh 'aws s3 ls s3://frontend002'
        sh 'aws s3 ls s3://frontend002/ --recursive'
        sh 'aws s3 ls s3://frontend002/ --recursive --human-readable --summarize'
    }
}
}
