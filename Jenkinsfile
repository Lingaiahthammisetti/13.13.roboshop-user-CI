@Library('jenkins-shared-library-for-roboshop')

// create variable of map type and set the values

def configMap = [ //We no need type, because we are calling pipeline directly.
    component: "user",
    project: "roboshop"
]
echo "test:"
if( ! env.BRANCH_NAME.equalsIgnoreCase('main')){
    nodeJSEKSPipeline(configMap)
}
else{
    echo "Proceed with CR or NON-PROD pipeline"
}