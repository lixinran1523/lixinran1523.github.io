# Research Experience Section Usage Guide

## Overview
I have added a new "Research Experience" section to your Jekyll academic website for showcasing your research projects and publications.

## New Files and Features

### 1. Configuration Updates
- `_config.yml`: Added `research_experience` collection configuration
- `_data/navigation.yml`: Added "Research Experience" link to navigation menu

### 2. New Directories and Files
- `_research_experience/`: Directory for storing research experience entries
- `_pages/research-experience.html`: Research experience main page
- `_includes/archive-single-research.html`: Specialized template for research experience display

### 3. Sample Files
Created 3 sample research experience files:
- `2024-01-01-research-project-1.md`: Deep Learning Applications in Medical Image Diagnosis
- `2023-06-01-research-project-2.md`: Natural Language Processing in Intelligent Question Answering Systems
- `2023-03-01-research-project-3.md`: Computer Vision Applications in Autonomous Driving

## How to Add New Research Experience

### 1. Create New Research Experience File
Create a new Markdown file in the `_research_experience/` directory with filename format: `YYYY-MM-DD-project-name.md`

### 2. File Header Configuration
Each research experience file should include the following YAML header information:

```yaml
---
title: "Project Title"
collection: research_experience
category: research
permalink: /research_experience/filename
excerpt: 'Project description'
date: YYYY-MM-DD
venue: 'Institution Name'
type: 'Project Type'
duration: 'Project Duration'
supervisor: 'Supervisor'
paperurl: '/files/paper.pdf'
---
```

### 3. File Content
Add detailed project description after the YAML header, including:
- Research background and objectives
- Key contributions and innovations
- Technical stack and implementation methods
- Project outcomes and impact

## Supported Download Link Types

- `paperurl`: Paper PDF file (prominently displayed with large green "View Paper" button)

The paper link will be displayed as a prominent button below each research experience entry for easy access to the PDF document.

## Custom Styling

If you need to adjust the styling of the research experience page, you can:
1. Modify the `_includes/archive-single-research.html` template
2. Add custom CSS styles in the `_sass/` directory

## Important Notes

1. Ensure PDF files are placed in the `files/` directory
2. Use English filenames with hyphens, avoid Chinese characters
3. Use YYYY-MM-DD date format
4. Each research experience entry will automatically generate a separate page

You can now visit the `/research-experience/` page to view the new Research Experience section!
