# Resources on fMRI and fMRI data analysis

Last updated: 2026-Feb-07

---

## Table of Contents

- [About](#about)
- [What is fMRI, and how does it work?](#what-is-fmri-and-how-does-it-work)
- [Courses](#courses)
- [Tools](#tools)
  - [FSL](#fsl)
  - [fMRIPrep](#fmriprep)
  - [FreeSurfer](#freesurfer)
  - [Nilearn / NiBabel / Nipype](#nilearn--nibabel--nipype)
- [Statistics](#statistics)
- [How to contribute?](#how-to-contribute?)
- [License](#license)

---

## About

Here are some useful resources about fMRI and fMRI data analysis with my non-useful comments. I prefer Python and work on Ubuntu Linux and use the Bash shell in the terminal. So far I've worked with FSL tools (such as BET, FAST, FIRST, and FSL-VBM) and fMRIPrep, Nilearn, and NiBabel, along with other Python libraries (such as NumPy, Pandas, Seaborn, Scipy, and Pingouin) for neuroimaging data analysis.

Most of the resources I've added here are because I've used those tutorials or worked on those tools. A few years ago, I had no idea about all this stuff, and these resources helped me in my learning journey. I maintain markdown files in Obsidian for my learning, and this page is one of them. Hopefully these resources will be helpful to you as well. On the Internet, there are countless materials. I tried to avoid providing links to the books or anything that is not free or easy to access. Different people have different learning styles. What worked for me may not necessarily work for you. If you've worked on some other tools or the same tools I've mentioned here and feel you have something to add, please feel free to do so. More descriptions about contributions have been provided at the bottom of the page; see [How to contribute?](#how-to-contribute?). Also, feel free to provide your suggestions or comments.

I tried to add specific stuff related to fMRI and fMRI data analysis, leaving out general introductions about cognitive neuroscience, the human brain, programming, and other relevant information. Though it's not quite possible to completely isolate fMRI from other relevant fields. You may find some overlap and integration with other areas of study. I may create another repo for general cognitive neuroscience topics or some specific topics (such as EEG or Python programming) if there is enough interest. I'll try to update this document on a regular basis if there are new updates to add.

**NOTE:** Standard neuroimaging analyses generally do not require a GPU. They are primarily designed to run on CPUs. High-core-count CPUs and large RAM are required for most cases. I've added some alternative tools, which require or highly recommend GPUs for performance.

---

## What is fMRI, and how does it work?
> Videos, animations, and lectures to introduce the science behind fMRI and how it is used in research.

01 [Understanding MRI: What is functional MRI (fMRI)?](https://youtu.be/4UOeBM5BwdY?si=1Ahl1BWqDa2Jvlfc)
> a good intro

02 [The Insane Engineering of MRI Machines](https://youtu.be/NlYXqRG7lus?si=J_IwJmG2D7RJYwQx)
> Great explanation about how MRI machines work along with superb visualizations.

03 [Brain Imaging, Crash Course](https://youtu.be/DdPRfPm9SI4?si=qWXv_X_NtGyVeKto)
> a detailed video

04 [Basics of fMRI](https://www.youtube.com/watch?v=-C84RFgyzuE) by Jamie Ward, University of Sussex

05 [Introduction to MRI of the brain](https://youtu.be/Co7Qyu21QKU?si=eq-Oeg1Z_EK9L-0N)

06 [Brain Signals: fMRI](https://youtu.be/8hhQGHYsXOY?si=gjDt0Z2GmH5NVWnb)

07 [How do we safely study living brains? - John Borghi and Elizabeth Waters - YouTube](https://www.youtube.com/watch?v=B10pc0Kizsc)
> TED-Ed animation video

08 [How does an MRI work? | MRI basics explained | Animation](https://www.youtube.com/watch?v=FvOezMIL9BU)

09 [MRI Physics | Magnetic Resonance and Spin Echo Sequences - Johns Hopkins Radiology](https://www.youtube.com/watch?v=jLnuPKhKXVM)

**Videos from Clover learning**
> 01 [What’s the difference between T1 and T2 relaxation? - MRI physics explained](https://www.youtube.com/watch?v=qrR2yoRhAmY)
> 
> 02 [T1, T2 and Proton Density Weighting explained - MRI physics](https://www.youtube.com/watch?v=7MN18gg1g_Y)
> 
> 03 [How does fMRI reveal which parts of the brain are active? - MRI physics explained - YouTube](https://www.youtube.com/watch?v=q7qoT2RhcDc)
> 
> 04 [Anatomical Planes - YouTube](https://www.youtube.com/watch?v=RmhPlBdn-Po)
> 
> 05 [MRI Cross Sectional Anatomy of the Brain (Sagittal View) - YouTube](https://www.youtube.com/watch?v=PlDrax1_sdY)
>
> This channel has so many more useful videos related to the diagnostic imaging field. I just added a few which were relevant to me, but there are plenty more to explore. Also, in the above mentioned list we've got two videos specifically about T1- and T2-weighted images.

**Series of lectures by Kevin Kang-Ik Cho, Harvard Medical School**
>01 [Learn this first for neuroimaging: Introduction to MRI neuroimaging data for Neuroscience | part 1](https://youtu.be/stuKESaa6Gs?si=fCokGuzgUEEC5Yza)
>
>02 [Look at Data First: Introduction to MRI Neuroimaging Data for Neuroscience | part 2](https://youtu.be/sEvr2PAw1Gc?si=PXyw6ZKxdlUczeJT)


### T1- and T2-weighted images

01 [T1 vs T2 weighted MRI images: How to tell the difference](https://www.youtube.com/watch?v=UKLvLsK36qo)

02 [MRI interpretation - T1 v T2 images](https://www.radiologymasterclass.co.uk/tutorials/mri/t1_and_t2_images)

---

## Courses
01 [Brainhack school](https://school-brainhack.github.io/)
> I was fortunate to take this course as part of my university curriculum. You can follow the modules and learn a lot. Brainhack School was a great starting point for me to learn a lot of things about programming and neuroimaging data analysis. I'm specifying here two modules related to fMRI. However, as I've already mentioned, there's much more to learn in Brainhack school. I encourage you to explore and take advantage of all the resources available.
> 
> // 01 [fMRI connectivity](https://school-brainhack.github.io/modules/fmri_connectivity/)
> // 02 [fMRI Parcellation](https://school-brainhack.github.io/modules/fmri_parcellation/)

02 [fMRI data analysis course taught at Nicolaus Copernicus University](https://github.com/fMRIAnalysisCourse/fmri-analysis-course?tab=readme-ov-file)
> I haven't done this course. Though it seems like it's quite structured, useful and specific about fMRI data analysis, along with necessary training in Python programming.

03 [Introduction to Working with MRI Data in Python: Summary and Setup](https://carpentries-incubator.github.io/SDC-BIDS-IntroMRI/)
> For beginners venturing into neuroimaging data handling, it's a promising and practical resource.

04 Series of lectures presented by Joram Soch, OvGU Magdeburg
> 01 [Lecture 1: "Preprocessing of fMRI Data" (Neuroimaging Lecture, SS 2023) - YouTube](https://www.youtube.com/watch?v=vcDm_fdNews)
>
> 02 [Lecture 2: "Statistical Analysis of fMRI Data" (Neuroimaging Lecture, SS 2023) - YouTube](https://www.youtube.com/watch?v=WRiNYGJMJps)
>
> 03 [Appendix 1: "Addendum to Preprocessing" (Neuroimaging Lecture, SS 2023)](https://www.youtube.com/watch?v=edxaeixs8k0)
>
> 04 [Appendix 2: "Addendum to Statistical Analysis" (Neuroimaging Lecture, SS 2023)](https://www.youtube.com/watch?v=ZVXZS5yKtUs)
>
> An updated version of Lecture 2
> 
> [Statistical Analysis of fMRI Data: The General Linear Model (Neuroimaging Lecture, SS 2024) - YouTube](https://www.youtube.com/watch?v=HTS1y0gRpes)

---

## Tools
### FSL
> FSL (FMRIB Software Library) is a comprehensive, open-source software suite developed at the University of Oxford for analyzing fMRI, structural, and diffusion-weighted brain imaging data. It provides command-line and GUI tools for preprocessing (e.g., motion correction, registration) and statistical modeling of brain activity.

01 fMRI Short Course with FSL
[Introduction — Andy's Brain Book 1.0 documentation](https://andysbrainbook.readthedocs.io/en/latest/fMRI_Short_Course/fMRI_Intro.html)
> You can't have a resource list about anything related to the human brain without Andy's Brain book. Brilliant tutorial to start with FSL.

02 [FSL - FMRIB Software Library](https://fsl.fmrib.ox.ac.uk/fsl/docs/index.html)
> New website for FSL

03 [FSL](https://fsl.fmrib.ox.ac.uk/fsl/oldwiki/)
> Old website for FSL. The new website is excellent, well structured, and elaborate. However, this old site is also quite informative.

04 [FSL Course](https://open.oxcin.ox.ac.uk/pages/fslcourse/website/index.html)
> FSL Course website. Go to the bottom of this page, and you'll be able to download PDF versions of three free short introductions. Those were pretty useful to me and great for someone who's new to this field. 
> 
> I read them in this order: 
> - 01 Short Introduction to Brain Anatomy for Neuroimaging
> - 02 Short Introduction to MRI Physics for Neuroimaging
> - 03 Short Introduction to the General Linear Model for Neuroimaging

05 [FSL Course Material](https://open.oxcin.ox.ac.uk/pages/fslcourse/website/online_materials.html)
> FSL Course Materials.

06 [Structural Analysis Practical](https://open.oxcin.ox.ac.uk/pages/fslcourse/practicals/seg_struc/index.html)
> Tutorials for FAST, FIRST, and FSL-VBM

07 [FSL course - BET — Neurodesk](https://neurodesk.org/example-notebooks/structural_imaging/FSL_course_bet.html)
> A better and interactive tutorial for BET based on the official FSL course.

---

### fMRIPrep
> fMRIPrep is an open-source, robust, and automated preprocessing pipeline designed to prepare raw, Brain Imaging Data Structure (BIDS)-formatted fMRI data for analysis. It minimizes manual intervention by combining tools from FSL, ANTs, FreeSurfer, and AFNI to perform essential tasks like motion correction, distortion correction, segmentation, and normalization.

01 [fMRIPrep: A Robust Preprocessing Pipeline for fMRI Data — fmriprep version documentation](https://fmriprep.org/en/stable/#)

02 [How much RAM/CPUs is reasonable to run pipelines like fmriprep? - Neuro Questions - Neurostars](https://neurostars.org/t/how-much-ram-cpus-is-reasonable-to-run-pipelines-like-fmriprep/1086)
> Even though this conversation is quite old, it's fairly useful.

03 [Running fMRIPrep on HPC — DartBrains](https://dartbrains.org/content/fmriprep_on_discovery.html)
> This is from a very useful course. It was helpful for my personal learning.

// Alternative tool
**DeepPrep** (for preprocessing), 
> which is a similar pipeline to fMRIPrep that recommends GPUs to leverage deep learning for faster processing.

01 [Welcome to DeepPrep’s documentation! — DeepPrep documentation](https://deepprep.readthedocs.io/en/latest/)

02 [DeepPrep: an accelerated, scalable and robust pipeline for neuroimaging preprocessing empowered by deep learning | Nature Methods](https://www.nature.com/articles/s41592-025-02599-1)
> a recent article about DeepPrep.   

---

### FreeSurfer
> I've never worked with FreeSurfer. However, for fMRI data preprocessing with fMRIPrep, you need a FreeSurfer license key. Also, if anyone has worked with FreeSurfer, please feel free to add resources related to it.

// Alternative tool
**FastSurfer** (for segmentation) 
> requires or highly recommends GPUs for performance.

---

### Nilearn / NiBabel / Nipype
> Nilearn, NiBabel, and Nipype are all essential Python libraries for fMRI analysis, but they serve different, complementary purposes within the neuroimaging ecosystem. They work together as part of the broader "nipy" (Neuroimaging in Python) ecosystem. 	
> 
> - NiBabel is a low-level library for reading, writing, and manipulating neuroimaging data formats like NIfTI (.nii or .nii.gz), DICOM, and GIFTI. 
> - Nilearn is a high-level library that offers tools for statistical analysis and machine learning with neuroimaging data, particularly fMRI. 
> - Nipype (Neuroimaging in Python Pipelines and Ecosystem) is a framework for creating and managing complex, reproducible analysis pipelines by providing a unified interface to existing software packages (like FSL, SPM, and ANTs) as well as other Python libraries (Nilearn, NiBabel).

01 [Neuroimaging in Python - Pipelines and Interfaces — nipy pipeline and interfaces package](https://nipype.readthedocs.io/en/latest/index.html#)

02 [Nilearn](https://nilearn.github.io/stable/index.html)

03 [Neuroimaging in Python — NiBabel 5.4.0.dev1+g3b1c7b37 documentation](https://nipy.org/nibabel/)

**Tutorials**

01 [MRI analysis in Python using Nipype, Nilearn and more](https://peerherholz.github.io/workshop_weizmann/index.html)
> Its structure, covering prerequisites, data handling, and advanced topics such as machine learning and connectivity analysis, makes it suitable for neuroimaging enthusiasts with basic programming knowledge.

02 [Functional Neuroimaging Analysis in Python: Summary and Setup](https://carpentries-incubator.github.io/SDC-BIDS-fMRI/)
> it's a solid, practical intro for researchers or students to brain imaging

03 [User guide - Nilearn](https://nilearn.github.io/stable/user_guide.html)

---

## Statistics
> crucial for effectively interpreting and representing our data

01 [Reporting Effect Sizes vs. T-Statistics in Neuroimaging](https://youtu.be/pPJyRh7_1EE?si=P8Wl5nx7q0L9Hg1F)

---

## How to contribute?

Suggestions and contributions are welcome:

- **New resources:** Tutorials, courses, or tools you found useful (especially free and accessible).  
- **Corrections:** Broken links, outdated descriptions, or mistakes.  
- **Other tools:** If you use different (or additional) tools and have good references, feel free to add them.

You can contribute by opening an issue or pull request. Suggestions and comments are always welcome.

---

## License

This repository is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You may share and adapt the material with appropriate credit. See the [LICENSE](LICENSE) file for the full legal code.
