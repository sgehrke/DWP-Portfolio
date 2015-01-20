Shaun Gehrke's Development Plan

# Deployment Plan

## Select Master Branch

### Merge Dev Branch into Master
	* $ git checkout master
	* $ git pull **github** master
	  * Resolve any conflicts

## Update Files

##### Make change to file
	* git add -A
	* git commit -m “detailed update note”

### Promote to Staging
	* $ git push staging 

### Test Staging
* Replicate any issues in local dev environment
* A new local dev branch may be needed to start over

### Promote to Production
* Have other users try it out prior to going live in production
* If no issues are present promote to Production server
	* git push LiveServer master
