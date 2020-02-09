# circleci
a practice of cricleci

# Variable	Type	Value
# CI	Boolean	true (represents whether the current environment is a CI environment)
# CI_PULL_REQUEST
	String	Deprecated version of CIRCLE_PULL_REQUEST. Kept for backward compatibility with CircleCI 1.0.
# CI_PULL_REQUESTS	
List	Deprecated version of CIRCLE_PULL_REQUESTS. Kept for backward compatibility with CircleCI 1.0.
# CIRCLE_BRANCH
	String	The name of the Git branch currently being built.
# CIRCLE_BUILD_NUM
	Integer	The number of the CircleCI build.
# CIRCLE_BUILD_URL
	String	The URL for the current build.
# CIRCLE_COMPARE_URL
	String	The GitHub or Bitbucket URL to compare commits of a build. Available in config v2 and below. For v2.1 we will introduce “pipeline values” as an alternative.
# CIRCLE_INTERNAL_TASK_DATA
	String	The directory where test timing data is saved.
# CIRCLE_JOB
	String	The name of the current job.
# CIRCLE_NODE_INDEX
	Integer	The index of the specific build instance. A value between 0 and (CIRCLE_NODE_TOTAL - 1)
# CIRCLE_NODE_TOTAL
	Integer	The number of total build instances.
# CIRCLE_PR_NUMBER
	Integer	The number of the associated GitHub or Bitbucket pull request. Only available on forked PRs.
# CIRCLE_PR_REPONAME
	String	The name of the GitHub or Bitbucket repository where the pull request was created. Only available on forked PRs.
# CIRCLE_PR_USERNAME
	String	The GitHub or Bitbucket username of the user who created the pull request. Only available on forked PRs.
# CIRCLE_PREVIOUS_BUILD_NUM
	Integer	The number of previous builds on the current branch.
# CIRCLE_PROJECT_REPONAME
	String	The name of the repository of the current project.
# CIRCLE_PROJECT_USERNAME
	String	The GitHub or Bitbucket username of the current project.
# CIRCLE_PULL_REQUEST
	String	The URL of the associated pull request. If there are multiple associated pull requests, one URL is randomly chosen.
# CIRCLE_PULL_REQUESTS
	List	Comma-separated list of URLs of the current build’s associated pull requests.
# CIRCLE_REPOSITORY_URL
	String	The URL of your GitHub or Bitbucket repository.
# CIRCLE_SHA1
	String	The SHA1 hash of the last commit of the current build.
# CIRCLE_TAG
	String	The name of the git tag, if the current build is tagged. For more information, see the Git Tag Job Execution.
# CIRCLE_USERNAME
	String	The GitHub or Bitbucket username of the user who committed the build.
# CIRCLE_WORKFLOW_ID
	String	A unique identifier for the workflow instance of the current job. This identifier is the same for every job in a given workflow instance.
# CIRCLE_WORKING_DIRECTORY
	String	The value of the working_directory key of the current job.
# CIRCLECI
	Boolean	true (represents whether the current environment is a CircleCI environment)
# HOME
	String	Your home directory.




<!-- ------------------------------------------------------------------------------ -->

# Running Your First CircleCI Build!
	You should see your build start to run automatically—and pass! So, what just happened? Click on the green Success button on the CircleCI dashboard to investigate the following parts of the run:

# Spin up environment: 
    CircleCI used the circleci/ruby:2.4.1 Docker image to launch a virtual computing environment.

# Checkout code: 
    CircleCI checked out your GitHub repository and “cloned” it into the virtual environment launched in Step 1.

# echo: 
    This was the only other instruction in your config.yml file: CircleCI ran the echo command with the input “A first hello” (echo, does exactly what you’d think it would do).