pipeline {
	agent any
	triggers {
		pollSCM("")
	}
	stages {
		stage("Build") {
			steps {
				upsertStack()
				upsertStack "Joel"
			}
		}
	}
}