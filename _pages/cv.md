Added both:
GO-BGC Float Data and Science Workshop, University of Washington, Seattle, August 17–21, 2026
Described you as a selected participant in the collaborative BGC-Argo data workshop.
GitHub under computing workflows alongside Linux, Git, and high-performance computing.
The workshop dates and location match the official GO-BGC listing.
Ok cool now how do I update the website 
The easiest method is through GitHub’s website. Your site automatically rebuilds whenever you commit changes to the repository.
1. Open your repository
Go to victoriaschoenwald/victoriaschoenwald.github.io and sign in.
2. Update the CV page
Open:
_pages → cv.md

Click the pencil icon, replace the existing contents with the updated CV page, then click Commit changes.

3. Update the publications page
Do the same for:
_pages → publications.md

Use the updated Publications page.

4. Replace the fake publications
Inside _publications, delete these three template files:
2009-10-01-paper-title-number-1.md
2010-10-01-paper-title-number-2.md
2015-10-01-paper-title-number-3.md
Then upload these two new files:
BAMS publication
Dissertation
To upload them, open _publications, select Add file → Upload files, and commit the upload.
5. Remove the fake PDFs
Inside the files folder, delete:
paper1.pdf
paper2.pdf
paper3.pdf
6. Check the deployment
After committing everything:
Open the repository’s Actions tab.
Wait for the Pages build to receive a green checkmark.
Visit victoriaschoenwald.github.io/cv and victoriaschoenwald.github.io/publications.
GitHub Pages can take a few minutes to display the changes.

cv.md
Document


publications.md
Document


2025-08-22-simplified-physics-agcm.md
Document

1 more
how do I replace the existing content with the updated CV page
Here’s the simplest way:
Download the updated cv.md file.
Open your GitHub repository:
victoriaschoenwald/victoriaschoenwald.github.io
Click the _pages folder, then click cv.md.
Click the pencil icon near the upper-right corner to edit the file.
Click inside the editing box and select everything:
Mac: Command + A
Windows: Ctrl + A
Press Delete, then open the downloaded cv.md on your computer and copy all its contents.
Paste the updated content into the GitHub editing box.
Click Commit changes… in the upper-right corner.
Enter a message such as:
Update CV page

Keep Commit directly to the master branch selected and click Commit changes.
After a few minutes, check victoriaschoenwald.github.io/cv.

cv.md
Document








cv.md


layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
/resume
Current position
Postdoctoral Researcher<br>
Kirtman Research Group, Rosenstiel School of Marine, Atmospheric, and Earth Science<br>
University of Miami
I study how climate change and natural variability influence regional sea-level rise and coastal flooding along the U.S. East Coast. My work combines observations, ocean and atmospheric reanalyses, and climate-model experiments to investigate the roles of atmospheric forcing, Gulf Stream variability, and large-scale climate dynamics.

Education
Ph.D., Atmospheric Sciences, University of Miami, 2025<br>
Dissertation: Understanding Regional Sea Level Rise Acceleration Along the North American Eastern Seaboard
B.S., Biology, Sacred Heart University
Research areas
Regional sea-level variability and change
Coastal ocean dynamics and flooding
Gulf Stream variability
Atmosphere–ocean interactions
Climate variability and predictability
High-resolution climate modeling
Research and technical skills
Scientific computing: Python, Jupyter, xarray, Dask, NumPy, SciPy
Analysis and visualization: Matplotlib, Cartopy, statistical analysis, time-series analysis, geospatial visualization
Climate and ocean data: tide gauges, satellite altimetry, atmospheric and ocean reanalyses, gridded observational datasets
Modeling: CESM, high- and low-resolution climate-model experiments, prescribed-forcing experiments
Computing workflows: Linux, Git, GitHub, high-performance computing, large multidimensional datasets
Workshops and professional development
GO-BGC Float Data and Science Workshop, University of Washington, Seattle, Washington, August 17–21, 2026<br>
Selected participant in a collaborative, hackathon-style workshop using BGC-Argo float data to address ocean biogeochemistry research questions.
Publications
{% include base_path %}
{% for post in site.publications reversed %}
{% include archive-single-cv.html %}
{% endfor %}

For a complete and current publication record, visit my [Google Scholar profile]({{ site.author.googlescholar }}).

Professional profiles
[Google Scholar]({{ site.author.googlescholar }})
[ORCID]({{ site.author.orcid }})
[ResearchGate]({{ site.author.researchgate }})
[GitHub](https://github.com/{{ site.author.github }})
