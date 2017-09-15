# Projects we are working on

We try to work as openly as possible. If you are interested in these problems or have solved any of these problems please contact us. For us a solution typically implies available data, code, and/or replicated results.



## neurodocker - generate custom dockerfiles

**Summary of question/problem:** Reproducibility is essential in science. Differences in computing environments have been shown to affect results of analyses (cite satra here), so these environments should themselves be reproducible by other groups. Containers can be used to package the software necessary to run an experiment or analyses into a single unit, but the creation of these containers is nontrivial. Neurodocker abstracts the installation details of each package from the user, making it much easier to create containers for neuroimaging. Specifically, Neurodocker generates Dockerfiles, which are the specifications used to create custom Docker images. These images can be created and used on any Linux, macOS, or Windows machine.

**Status:** ongoing but reaching stability

**Collaborators:** Satra Ghosh, MIT

**Repo:** [kaczmarj/neurodocker](https://github.com/kaczmarj/neurodocker)

**Issue link to discuss:** na

**Estimated timeline:**: release stable api (ie, v1.0) sometime in October.



## nobrainer - segmentation of brains (and later tumors) with neural networks

**Summary of question/problem:** Neural networks can be used to segment meaningful parts of images. Can we train a neural network to segment brains in 2-dimensional, anatomical slices? Can we train a neural network to segment globular tumors (i.e., meningioma) in 2-dimensional, anatomical slices? Can we segment in 3 dimensions? This will provide an alternative method of brain extraction that could improve upon existing tools.

**Status:** ongoing

**Collaborators:** Satra Ghosh (MIT) and Omar Arnaout (BWH)

**Repo:**
- [kaczmarj/nobrainer](https://github.com/kaczmarj/nobrainer)
- [kaixiw/MeningiomaSegmentation](https://github.com/kaixiw/MeningiomaSegmentation) (previous work)

**Issue link to discuss:** na

**Estimated timeline:** by end of 2017




## nipype testing

**Summary of question/problem:** The time it takes to run Nipype's tests on CircleCI can be shortened with the use of Neurodocker, ReproZip, and CircleCI's built-in caching.

**Status:** Ongoing

**Collaborators:** Nipype developers

**Repo/Document/Details:** [kaczmarj/nipype@enh/circleci-neurodocker](https://github.com/kaczmarj/nipype/tree/enh/circleci-neurodocker)

**Issue Link to discuss:** [nipy/nipype#2144](https://github.com/nipy/nipype/issues/2144)

**Estimated timeline:** by end of September


<!--
## Problem X

**Summary of question/problem:**

**Status:** Completed/On going/Set aside/

**Collaborators:**

**Repo/Document/Details:** https://example.org

**Issue Link to discuss:** https://example.org

**Estimated timeline:** By end of 2233
-->
