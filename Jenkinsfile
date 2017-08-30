pipeline {
	agent any
	triggers {
		pollSCM("")
	}
	stages {
		stage("Build") {
			steps {
				echo "Before upsertStack"
				upsertStack("Joel", ["P1Key":"P1Value", "P1Key":"P1Value"])
				echo "After upsertStack"
			}
		}
	}
}