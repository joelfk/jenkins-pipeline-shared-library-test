pipeline {
	agent any
	triggers {
		pollSCM("")
	}
	stages {
		stage("Build") {
			steps {
				upsertStack stackName: "Joel" parameters: ["P1Key":"P1Value", "P1Key":"P1Value"]
			}
		}
	}
}