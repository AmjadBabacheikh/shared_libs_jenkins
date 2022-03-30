# shared_libs_jenkins
Demo describing shared library in jenkins

After configuring shared library in jenkins we can use in the pipeline:
```
@Library("jenkins-lib-demo") _

pipeline{
    agent any
    stages{
        stage("calling shared library"){
        steps{
            script{
            shared.call("amjad")
            shared.sum(5,9)
                
            }
        }
    }
  }
    
}
```
