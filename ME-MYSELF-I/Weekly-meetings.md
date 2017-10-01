# Weekly Meetings

* [22nd September 2017](#date-22nd-september-2017)
* [14th September 2017](#date-14th-september-2017)


### Date: 22nd September 2017

#### Who did you help this week?

I helped (and am in the process of helping) the ReproZip team streamline their Dockerfile and develop methods to minimize Docker containers (see [ViDA-NYU/reprozip#274](https://github.com/ViDA-NYU/reprozip/issues/274)). I also helped Dorota [@djarecka](https://github.com/djarecka) debug a workflow that uses Common Workflow Language.

#### Who helped you this week?

[Satra](https://github.com/satra) helped me by providing guidelines for regression testing and by linking me to existing networks for brain image segmentation. Dorota [@djarecka](https://github.com/djarecka) helped me by introducing me to Common Workflow Language syntax.

#### What did you achieve?

* Created [a matrix of Docker images](https://hub.docker.com/r/kaczmarj/regtests/tags/) to test with [ReproNim/simple_workflow](https://github.com/ReproNim/simple_workflow).
  * Tested simple_workflow in an FSL 5.0.10 Docker container, and minified that container for the workflow.
* Downloaded BrainBox NIFTI files to OpenMind. These files will be used to train/test a net for nobrainer.
* Neurodocker bug fixes.

#### What did you struggle with?

* Training a neural net on the BrainBox NIFTI data. I had difficulty organizing the data in the form required for each net.

#### What would you like to work on next week?

* Train/test a neural net on BrainBox NIFTI data.
* Submit a work-in-progress PR to nipype to update their testing with CircleCI 2.0.
* Add support for FSL eddy 5.0.11 to Neurodocker.



### Date: 14th September 2017

#### Who did you help this week?

I helped GitHub user [@sulantha2006](https://github.com/sulantha2006) by reviewing and accepting his pull request to add MINC and PETPVC to Neurodocker, and I helped Mathias ([@mgxd](https://github.com/mgxd)) scan for the Voice study.

#### Who helped you this week?

Dorota ([@djarecka](https://github.com/djarecka)) helped me think of ways to test different versions of FSL with Neurodocker.

#### What did you achieve?

* Added features to Neurodocker to be able to generate Dockerfiles for Nipype, and fixed bugs.
* Drafted at least two potential workflows for Nipype testing on CircleCI.

#### What did you struggle with?

* Implementing a Nipype testing workflow.

#### What would you like to work on next week?

* Submit a job on openmind to train a neural network based on a semantic segmentation paper (I will add the citation soon). This should take several hours, but once this is done, it should be quicker to submit training jobs in the future.
* Implement a Nipype testing workflow on CircleCI, and submit a "work in progress" pull request to nipype.


<!--
## Template (Copy template, add date link on top, and replace text, newest first)

### Date: [INSERT DATE OF MEETING]

#### Who did you help this week?

Replace this text with a one/two sentence description of who you helped this week and how.

#### Who helped you this week?

Replace this text with a one/two sentence description of who helped you this week and how.

#### What did you achieve?

* Replace this text with a bullet point list of what you achieved this week.
* It's ok if your list is only one bullet point long!

#### What did you struggle with?

* Replace this text with a bullet point list of where you struggled this week.
* It's ok if your list is only one bullet point long!

#### What would you like to work on next week?

* Replace this text with a bullet point list of what you would like to work on next week.
* It's ok if your list is only one bullet point long!
* Try to estimate how long each task will take.

#### Any other topics

This space is yours to add to as needed.
-->
