pipeline {
	agent any
	triggers {
		pollSCM("")
	}
	environment { 
        PARAM_VALUE = "P2Value"
    }
	stages {
		stage("Build") {
			environment { 
				ENV = "UAT"
			}
			steps {
				echo "Before upsertStack"
				upsertStack(
					stackName: "Joel",
					parameters: [
						"P1Key" : "P1Value",
						"P2Key" : ${env.PARAM_VALUE}
					])
				echo "After upsertStack"
			}
		}
	}
}