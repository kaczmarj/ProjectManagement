# Weekly Meetings

* [10th November 2017](#date-10th-november-2017)
* [3rd November 2017](#date-3rd-november-2017)
* [27th October 2017](#date-27th-october-2017)
* [20th October 2017](#date-20th-october-2017)
* [10th October 2017](#date-10th-october-2017)
* [6th October 2017](#date-6th-october-2017)
* [29th September 2017](#date-29th-september-2017)
* [22nd September 2017](#date-22nd-september-2017)
* [14th September 2017](#date-14th-september-2017)


### Date: 10th November 2017

#### Who did you help this week?

I helped Dorota use Neurodocker and Docker.

#### Who helped you this week?

Dorota contributed examples to Neurodocker.

#### What did you achieve?

- Nobrainer: ready to train niftynet's highres3dnet on gablab's aparc+aseg.mgz volumes (I've created a text file with all of gablab's apac+aseg.mgz filepaths and have a niftynet config file ready).
- Polished and optimized [nipype testing pull request](https://github.com/nipy/nipype/pull/2202).
- Analyzed behavioral and eeg data for Kana.
- Neurodocker bug fixes.

#### What did you struggle with?

- Nobrainer: using niftynet's pre-trained BRATS model to infer labels of the brainbox meningioma data.

#### What would you like to work on next week?

- Nobrainer: train highres3dnet on aparc+aseg.mgz volumes. infer labels on Mindboggle 101 data using highres3dnet model trained on gablab's aparc+aseg data. This will be my priority this week.
- Neurodocker: work on paper outline, and run regression tests. Will write outline and manuscript in [this Google Doc](https://docs.google.com/document/d/1_gval2-mXmMd8YXdMX9I-eNThE9oONzQrMG2l-53SUY/edit?usp=sharing).



### Date: 3rd November 2017

#### Who did you help this week?

I helped Dorota create a container for a Nipype tutorial. I also helped Hannah debug a PsychoPy script.

#### Who helped you this week?

Satra gave me advice on the Neurodocker refactor.

#### What did you achieve?

- Almost completed the Nipype testing pull request.
- Made progress on Neurodocker refactor. Learned more about [packer](https://www.packer.io/) and how neurodocker might interface with it.

#### What did you struggle with?

- Nipype testing PR is taking longer than expected.

#### What would you like to work on next week?

- Neural networks: train niftynet model on gablab's aparc+aseg data. Test that trained model on the mindboggle 101 dataset.
- Run regression tests on an FSL workflow. Create a dashboard of results.



### Date: 27th October 2017

#### Who did you help this week?

I helped Kana run an EEG experiment and analyze the data. I also helped Hannah with a PsychoPy script she wrote from scratch.

#### Who helped you this week?

Satra helped me prioritize my tasks and conceptualize the neurodocker paper.

#### What did you achieve?

- Kana and I collected EEG data from about 140 people, and we analyzed about half of it.
- I have also started refactoring neurodocker to make it easier for users to contribute "recipes."
- Made progress on the nipype testing pull request.

#### What did you struggle with?

- Checking whether commands being traced with reprozip failed. At the moment, `reprozip trace` will return code 0 even if a traced command fails. [ViDA-NYU/reprozip#281](https://github.com/ViDA-NYU/reprozip/pull/281) is in progress to fix this.

#### What would you like to work on next week?

- complete the nipype testing pull request
- neurodocker refactor
- outline the neurodocker paper
- train a niftynet model on all of gablab's aparc+aseg data, and test that trained model on the mindboggle 101 dataset.
- create a pure tensorflow/keras version of a niftynet model



### Date: 20th October 2017

#### Who did you help this week?

I helped Nick with analysis of a voxel-wise correlation map of real data and of shuffled data. I also helped a new OpenMind user with general OpenMind use and with Matlab/SPM.

#### Who helped you this week?

[@Shotgunosine](https://github.com/Shotgunosine) submitted enhancements for the AFNI installation in Neurodocker (added option to install system python2 and/or python3, not part of miniconda environment). Satra also helped me by having me sit in on meetings regarding a potential project.

#### What did you achieve?

* Analyzed wireless EEG data from a pilot study.
* Added `dcm2niix` support to Neurodocker (Neurodocker now listed on `dcm2niix`'s readme).

#### What did you struggle with?

* Finding the time to infer labels with NiftyNet.

#### What would you like to work on next week?

* I am at a conference for Sunday-Wednesday next week helping collect wireless EEG data.
* Infer labels with NiftyNet.
* Finish Nipype testing PR.



### Date: 10th October 2017

#### Who did you help this week?

I helped one group within the Gab Lab with their shared OpenMind environment (multiple users `conda install`ing created symlinks in `/home` that resulted in permissions issues). We resolved the issue, and we plan to meet with Mario to hold a workshop to create a singularity container for the project. That would be a better, more permanent solution.

#### Who helped you this week?

The Medulina team helped me this week by explaining to me the goals of the project and where I fit in. Three fantastic participants (from the Gab Lab) helped Kana and me pilot a wireless EEG exeriment.

#### What did you achieve?

* Trained a highres3dnet neural net on part of the camcan data. Have not inferred labels yet.
* Prepared analysis scripts for a wireless EEG experiment.
* Networked with folks in the AI space and learned from them about semantic segmentation.

#### What did you struggle with?

* Inferring labels with the trained highres3dnet. I will have to read the niftinet documentation more carefully.

#### What would you like to work on next week?

* Infer labels with highres3dnet. Potentially train other models on the camcan data.
* Add `dcm2niix` support to Neurodocker.



### Date: 6th October 2017

#### Who did you help this week?

I helped [danjgale](https://github.com/danjgale) use neurodocker to create a container for MR image analysis, and I helped openmind user brando90 work out his singularity and python issues.

#### Who helped you this week?

Dorota submitted a pull request to neurodocker (merged). [remram44](https://github.com/remram44) (creator of reprozip) discussed with me how to package reprozip in a standalone container and trace a process in a separate container (mindblowing).

#### What did you achieve?

* Inferred labels of gray/white matter + subcortical structures on brainbox data using a pre-trained niftynet model.
* Made progress modifying reprozip to trace a process within a container without having to install reprozip inside that container.
* Neurodocker improvements.

#### What did you struggle with?

* Writing C for reprozip.

#### What would you like to work on next week?

* Apply niftynet models to other data.
* Try to generate brains with niftynet's variational autoencoder.
* Work on minimizing a container without having to install reprozip in the container.
* Finish up my nipype testing PR.



### Date: 29th September 2017

#### Who did you help this week?

I helped [@sitek](https://github.com/sitek) create a Singularity container for DSI-Studio. (We are still trying to work out issues with libGL) [@mgxd](https://github.com/mgxd) and I helped Nick Hubbard shuffle the timeseries of each voxel in an fMRI recording. I also helped Nick run a Singularity container with the latest version of AFNI, and it looks like we discovered a bug in AFNI's version information.

#### Who helped you this week?

[StackOverflow user Divakar helped me](https://stackoverflow.com/a/46476164/5666087) improve the efficiency of code I wrote to shuffle the timeseries of each voxel in a 4-dimensional array. [@mgxd](https://github.com/mgxd) helped me incorporate that code into a nipype workflow. [@ross-mitchell](https://github.com/ross-mitchell) discovered and patched a bug in neurodocker's installation of AFNI.

#### What did you achieve?

* Created a local "webapp" for use in one of Kana's experiments.
* Taught Nick about containers and how to use them on openmind.

#### What did you struggle with?

* Time management. I had an exam during the middle of my week, and studying consumed much of my time. I'm hoping to catch up this upcoming week.

#### What would you like to work on next week?

* Train/test NiftyNet on the BrainBox data (should take a few hours to set up, not sure how long to run).
* Submit a work-in-progress PR to Nipype to update its CircleCI testing (should take an hour or less; most of the `config.yml` is written).
* Tackle open Neurodocker issues and PRs.



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
