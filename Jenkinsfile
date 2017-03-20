
node {
 
    // Mark the code checkout 'Checkout'....
    stage 'Checkout'
 
    // Get some code from a GitHub repository
    git url: 'https://github.com/atul-ram/web.git'
stage 'test'
        parallel (
            phase1: { sh "echo p1; sleep 2s; echo phase1" },
            phase2: { sh "echo p2; sleep 4s; echo phase2" }
        )

   stage name: 'validate', concurrency: 1
        sh "/usr/bin/packer validate project.json"
 sh "pwd"

 }
