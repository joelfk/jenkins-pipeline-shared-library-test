pipeline {
	agent any
	triggers {
		pollSCM("")
	}
	stages {
		stage("Build") {
			steps {
				echo "Before upsertStack"
				upsertStack stackName: "Joel"
				echo "After upsertStack"
			}
		}
	}
}