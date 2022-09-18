pipeline{
    agent any
    parameters{
        choice(Name: 'Version',choices: ['1.2','1.3','1.4'],Description:'')
    }
    stages{
        stage("Build"){
            steps{ 
                when{
                  expression{
                     params.Version
                }
            }
                echo "Build the stage"
                params.Str
            }
            }
stage("Test")
{
    steps{
        echo "show the version: ${Version}"
    }
}
    }
    
}
