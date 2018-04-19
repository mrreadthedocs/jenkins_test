node('master'){

stage("Test"){
    echo "test"
}

stage("Promote to master"){
    if (${env.BRANCH_NAME}=='develop'){
        echo "I am a develop brach!"
    }
}

}
