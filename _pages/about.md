---
permalink: /
title: "Introduction"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am associate professor at the Department of Computer Science and Engineering, School of Engineering and Architecture, University of Bologna. My research concerns computer vision and primarily focuses on scene perception with monocular, stereo, and multi-view setups and sensor fusion between LiDARs/ToFs and cameras. I’m IEEE Senior member.

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, Academic Pages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over - just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this template](https://github.com/academicpages/academicpages.github.io) by clicking the "Use this template" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

Publications
------
Journal articles

[J36] F. Tosi, F. Aleotti, P. Zama Ramirez, M. Poggi, S. Salti, S. Mattoccia, L. Di Stefano, “Neural Disparity Refinement”, IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), 2024 [PDF](https://doi.ieeecomputersociety.org/10.1109/TPAMI.2024.3411292)

[J35] X. Qiao, M. Poggi, P. Deng, H. Wei, C. Ge, S. Mattoccia, “RGB Guided ToF Imaging System: A Survey of Deep Learning-based Methods”, International Journal of Computer Vision (IJCV), 2024 [PDF | Arxiv]

[J34] M. Poggi, F. Arrigoni, A. Fusiello, S. Mattoccia, A. Bartoli, T. Sattler, T. Pajdla, “Guest Editorial: Special Issue on Traditional Computer Vision in the Age of Deep Learning”, International Journal of Computer Vision (IJCV), 2024 [PDF]

[J33] P. Zama Ramirez, A. Costanzino, F. Tosi, M. Poggi, S. Salti, S. Mattoccia, L. Di Stefano, “Booster: a Benchmark for Depth from Images of Specular and Transparent Surfaces”, IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), Volume: 46, Issue 1, pages: 85 - 102, January 2024 [PDF | Arxiv]

[J32] X. Qiao, C. Ge, Y. Zhang, Y. Zhou, F. Tosi, M. Poggi, S. Mattoccia, “Depth Super-Resolution from Explicit and Implicit High-Frequency Features”, Computer Vision and Image Understanding (CVIU), Volume 237, December 2023, 103841 [PDF | Arxiv]

[J31] X. Qiao, C. Ge, C. Zhao, F. Tosi, M. Poggi, S. Mattoccia, “Self-supervised Depth Super-resolution with Contrastive Multiview Pre-training”, Neural Networks (NN), Volume 168, November 2023, Pages 223-236 [PDF | Arxiv]

[J30] X. Qiao, C. Ge, P. Deng, H. Wei, M. Poggi, S. Mattoccia, “Depth Restoration in Under-Display Time-of-Flight Imaging”, IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), Volume 45, Issue 5, pages: 5668 - 5683, May 2023 [PDF]

[J29] P. Kaniewski, M. Pasternak, S. Mattoccia, “Special issue on Multi-Sensor Systems and Data Fusion in Remote Sensing", Remote Sensing, March 2023 [PDF | Book]

[J28] A. Mingozzi, A. Conti, F. Aleotti, M. Poggi, S. Mattoccia, “Monitoring social distancing with single image depth estimation”, IEEE Transactions on Emerging Topics in Computational Intelligence (TETCI), Volume 6, Issue 6, pages 1290 - 1301, December 2022 [PDF | Arxiv | Dataset]

[J27] M. Poggi, F. Tosi, F. Aleotti, S. Mattoccia, “Real-time monocular depth estimation without GPU”, IEEE Transactions on Intelligent Transportation Systems (T-ITS), Volume 23, Issue 10, pages 17342 - 17353, October 2022 [PDF | Video | Code]

[J26] M. Poggi, F. Tosi, K. Batsos, P. Mordohai, S. Mattoccia, “On the synergies between machine learning and binocular stereo for depth estimation from images: a survey”, IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), Volume 44, Issue 9, pages 5314 - 5334, September 2022 [PDF | Arxiv]

[J25] M. Poggi, S. Kim, F. Tosi, S. Kim, F. Aleotti, D. Min, K. Sohn, S. Mattoccia , “On the confidence of stereo matching in a deep-learning era: a quantitative evaluation”, IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), Volume 44, Issue 9, pages 5293 - 5313, September 2022 [PDF | Arxiv | Code]

[J24] M. Poggi, A. Tonioni, F. Tosi, S. Mattoccia, L. Di Stefano, “Continual adaptation for deep stereo”, IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), Volume 44, Issue 9, pages 4713 - 4729, September 2022 [PDF | Arxiv | Video | Code]

[J23] A. Cipolletta, V. Peluso, A. Calimera, M. Poggi, F. Tosi, F. Aleotti, S. Mattoccia, “Energy-Quality Scalable Monocular Depth Estimation on Low-Power CPUs”, IEEE Internet of Things Journal (IoT-J), Vol. 9, Issue 1, pages 25-36, January 1, 2021 [PDF]

[J22] V. Peluso, A. Cipolletta, A. Calimera, M. Poggi, F. Tosi, F. Aleotti, S. Mattoccia, “Monocular depth perception on microcontrollers for edge applications”, IEEE Transactions on Circuits and Systems for Video Technology (TCSVT), Vol. 32, Issue 3, pages 1524-1536, March 2022 [PDF | Video]

[J21] D. De Gregorio, M. Poggi, P. Zama Ramirez, G. Palli, S. Mattoccia, L. Di Stefano, “Beyond the baseline: 3D reconstruction of tiny objects with single camera stereo robot”, IEEE Access, Vol. 9, pages 119755 - 119765, August 2021 [PDF | Video]

[J20] F. Aleotti, G. Zaccaroni, L. Bartolomei, M. Poggi, F. Tosi, S. Mattoccia, “Real-time single image depth perception in the wild with handheld devices”, Sensors 2021, 21(1), 15; [PDF | Video_1 | Video_2 | Video_3 | Demo | Code]

[J19] A. Livoroi, A. Conti, L. Foianesi, F. Tosi, F. Aleotti, M. Poggi, F. Tauro, E. Toth, S. Grimaldi, S. Mattoccia, “On the deployment of out-of-the-box embedded devices for self-powered river surface flow velocity monitoring at the edge”, Applied Sciences 2021, 11(15), 7027 [PDF]

[J18] P. Tassinari, M. Bovo, S. Benni, S. Franzoni, M. Poggi, L. Maria, E. Mammi, S. Mattoccia, L Di Stefano, F. Bonora, A. Barbaresi, E. Santolini, D. Torreggiani, “A computer vision approach based on deep learning for the detection of dairy cows in free stall barn”, Computers and Electronics in Agriculture, Volume 182, March 2021, [PDF]

[J17] A. Tonioni, M. Poggi, S. Mattoccia, L. Di Stefano, “Unsupervised domain adaptation for depth prediction from images”, IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), 42(10), pages 2396 - 2409, October 1, 2020, 10.1109/TPAMI.2019.2940948, [PDF | Arxiv | Video | Code]

[J16] M. Poggi, F. Tosi, S. Mattoccia, “Good cues to learn from scratch a confidence measure for passive depth sensors”, IEEE Sensors Journal, 20(22), pages 13533-13541, November 15, 2020, DOI: https://doi.org/10.1109/JSEN.2020.3004629, [PDF | Arxiv] 

[J15] F. Tosi, M. Rocca, F. Aleotti, M. Poggi, S. Mattoccia, F. Tauro, E. Toth, S. Grimaldi, “Enabling image-based streamflow monitoring at the edge”, Remote Sensing, 2020, 12(12), 2047 [PDF]

[J14] M. Poggi, F. Tosi, S. Mattoccia, “Learning a confidence measure in the disparity domain from O(1) features”, Computer Vision and Image Understanding, Volume 193, April 2020 [PDF | Code]

[J13] M. Poggi, G. Agresti, F. Tosi, P. Zanuttigh, S. Mattoccia, “Confidence estimation for ToF and stereo sensors and its application to depth data fusion”, IEEE Sensors Journal, 20(2), pages 1411-1421, February, 1 2020 [PDF | PDF(Pre-Print) | Code]

[J12] F. Tauro, F. Tosi, S. Mattoccia, E. Toth, R. Piscopia, S. Grimaldi, "Optical Tracking Velocimetry (OTV): leveraging optical flow and trajectory-based filtering for surface streamflow observations", Remote Sensing, 2018, 10(12), 2010 [PDF | Video]

[J11] S. Mattoccia, B. Kisačanin, M. Gelautz, S. Chai, A. N. Belbachir, G. Dedeoglu, F. Stein, “Special issue on Embedded Computer Vision”, Journal of Signal Processing Systems, June 2018, Volume 90, Issue 6, pages 873–876 [PDF]

[J10] W. Ouyang, F. Tombari, S. Mattoccia, L. Di Stefano, W. Cham, "Performance evaluation of full-search equivalent pattern matching algorithms", IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), 34(1), pages 127-143, January 2012 [PDF | Bibtex]

[J9] A. Alatan, J. Ostermann, L. Onural, G. AlRegib, S. Mattoccia, C. Yuan, “Special issue on Emerging Techniques in 3-D”, IEEE Journal of Selected Topics in Signal Processing, Vol. 6, Num. 5, September 2012  [PDF]

[J8] S. Mattoccia, F. Tombari, L. Di Stefano, "Efficient template matching for multi-channel images", Pattern Recognition Letters (PRL), 32(5), pages 694-700, April 2011 [PDF | Bibtex]

[J7] F. Tombari, S. Mattoccia, L. Di Stefano, "Full search-equivalent pattern matching with Incremental Dissimilarity Approximations", IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), 31(1), pages 129-141, January 2009 [PDF | Bibtex]

[J6] S. Mattoccia, F. Tombari, L. Di Stefano, "Fast  full-search equivalent template matching by Enhanced Bounded Correlation", IEEE Transactions on Image Processing (TIP), 17(4), pages 528-538, April 2008 [PDF | Bibtex]

[J5] L. Di Stefano, S. Mattoccia, F. Tombari, “ZNCC-based template matching using Bounded Partial Correlation", Pattern Recognition Letters (PRL), 16(14), pages 2129-2134 October 2005 [PDF | Bibtex]

4 L. Di Stefano, M. Marchionni, S. Mattoccia, “A fast area-based stereo matching algorithm”, Image and Vision Computing (IVC), 22(12), pages 983-1005, October 2004 [PDF | Bibtex]

[J3] L. Di Stefano, M. Marchionni, S. Mattoccia, "A PC-based real-time stereo vision system", Machine Graphics & Vision, 13(3), pages 197-220, January 2004 [PDF | Bibtex]

[J2] L. Di Stefano, S. Mattoccia, “Fast template matching using Bounded Partial Correlation”, Machine Vision and Applications (MVA), 13(4), pages 213-221,  February 2003 [PDF | Bibtex]

[J1] L. Di Stefano, S. Mattoccia, “Real-time stereo within the VIDET project”, Real-Time Imaging (RTI), 8(5), pages 439-453, October 2002 [PDF | Bibtex]
