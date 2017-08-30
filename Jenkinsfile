pipeline {
	agent any
	triggers {
		pollSCM("")
	}
	stages {
		stage("Build") {
			steps {
				echo "Before upsertStack"
				upsertStack "Joel"
				echo "After upsertStack"
			}
		}
	}
}