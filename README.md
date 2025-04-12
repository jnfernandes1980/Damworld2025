# Damworld2025 - Using HEC-RAS for dam break simulation - Case Study

Welcome to this tutorial for the lecture on dam break simulation. 
It will guide you and cover the main steps to get the inundation due to a breach in a dam.
These are the main components:
![image](https://github.com/user-attachments/assets/470b280e-6676-489a-80e2-f6a7078227a4)

This is the current User Interface of HEC-RAS:
![image](https://github.com/user-attachments/assets/393f1d6a-71f0-46d7-aea4-75b10936c332)

Besides other functionalities, the most important sections are #Geometric data, #Simulations and #RAS Mapper

# STEP 0: Get terrain data

Download Elevation Data https://search.earthdata.nasa.gov/search

1. Register
2. Choose the area that is important for you
3. Download SRTM (1 sec arc in tif format)
  
   ![image](https://github.com/user-attachments/assets/9e5ddcee-ceae-4aff-b4bf-0868e8351ec0)

# STEP 1: Create terrain

1. In RAS Mapper - Add projection (https://spatialreference.org/)
2. Add new terrain with downloaded data (if you have more than one data set, order it. Put in the top the most relevant (LiDAR for the river and SRTM for the floodplains, for example) 
3. Create terrain
   
   ![image](https://github.com/user-attachments/assets/6e825357-2ded-46f2-885c-8c815e2af5c5)
Register

# STEP2:Create Storage Area (It will be your reservoir)

1. In RAS Mapper

2. Add new storage area

![image](https://github.com/user-attachments/assets/8ebd8ff7-8314-49b0-a84f-03ae3bd38780)
![image](https://github.com/user-attachments/assets/4eb3a4a1-1d37-4947-ab12-4c54ed3bdb58)


# STEP3:Create Connection storage area - 2d mesh (It will be the dam you want to breach)





![image](https://github.com/user-attachments/assets/4a8384bd-8a44-4094-9fdc-8f0af32edb16)

![image](https://github.com/user-attachments/assets/803a33fe-9d1f-4c1a-b97f-5b70872582b8)
Use this data for our case study
6. a GitHub account if you don't have one and confirm your e-mail (required!)
1. Click the "Use this template" button in the top right.
1. On the "New repository" page, enter your repository name as "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and add your content.
1. Upload any files (like PDFs, .zip files, etc.) to the `files/` directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section
1. (Optional) Use the Jupyter notebooks or python scripts in the `markdown_generator` folder to generate markdown files for publications and talks from a TSV file.

See more info at https://academicpages.github.io/

## Running Locally

When you are initially working your website, it is very useful to be able to preview the changes locally before pushing them to GitHub. To work locally you will need to:

1. Clone the repository and made updates as detailed above.
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `jekyll serve -l -H localhost` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.


# Maintenance 

Bug reports and feature requests to the template  should be [submitted via GitHub](https://github.com/academicpages/academicpages.github.io/issues/new/choose). For questions concerning how to style the template, please feel free to start a [new discussion on GitHub](https://github.com/academicpages/academicpages.github.io/discussions).

This repository was forked (then detached) by [Stuart Geiger](https://github.com/staeiou) from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License (see LICENSE.md). It is currently being maintained by [Robert Zupko](https://github.com/rjzupkoii) and additional maintainers would be welcomed.

## Bugfixes and enhancements

If you have bugfixes and enhancements that you would like to submit as a pull request, you will need to [fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo) this repository as opposed to using it as a template. This will also allow you to [synchronize your copy](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) of template to your fork as well.

Unfortunately, one logistical issue with a template theme like Academic Pages that makes it a little tricky to get bug fixes and updates to the core theme. If you use this template and customize it, you will probably get merge conflicts if you attempt to synchronize. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch.

