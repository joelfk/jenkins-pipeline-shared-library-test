pipeline {
	agent any
	triggers {
		pollSCM("")
	}
	stages {
		stage("Build") {
			steps {
				echo "Before upsertStack"
				upsertStack name: 'Joel'
				echo "After upsertStack"
			}
		}
	}
}