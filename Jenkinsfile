pipeline{
agent any
stages{
    
    stage("maven build"){
        when{
        branch "dev"
        }
        steps{
            echo "maven build!"
        }
    }
    
    stage("deploy to dev"){
        when{
        branch "dev"
        }
        steps{
            echo "deploying to dev!"
        }
    }
    
    stage("deploy to test"){
        when{
        branch "test"
        }
        steps{
            echo "deploying to test!"
        }
    }
    
    stage("deploy to production"){
        when{
        branch "main"
        }
        steps{
            echo "deploying to production!"
        }
    }
}
}