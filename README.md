# Assignment 1: Custom SPA Framework

## Overview

Using the SPA framework as a starting point, create a three `Page` application for the Humber Media Pros website. This site will be a Student-to-Employer site (or College-to-Employer, where we might send this url to a prospective employer on your behalf). The focus should be on showcasing student work and the core technologies learned in the program, as well as providing contact information for the student so you may be contacted for employment.

Each of the pages will represent the HTML template for one of: 

- **Home**: A generic homepage (may just be static)
- **Program**: Represents one of the three programs offered
- **Students**: Represents all students of a given program
  - may instead be included on the _Program_ page itself
- **Student**: Represents the content for one student 

## Goals

1. Understand the basics of a single page application
2. Learn to manage and develop a project collaboratively

## Getting started

1. In a group of 3 or 4, plan the content for each of the three pages above
1. Create a Github Organization for your team
1. Create a repo named after your organization in this format: `[orgname].github.io` (where `[orgname]` is replaced by your organization name)
1. Give access to the entire Organization (or just the Repo) to your team members
1. Create a README file with the following in it and commit to `master`:
	```
	# Humber Media Pros

	## Group
	```
1. Each member should write a ticket reminding themselves to "Add my name to the README.md"
   1. Assign it to yourself
   1. Add at least one "label" to the issue (use the most appropriate one)
1. Each member should now clone the repo, create a unique branch, and in that branch, add their name under the `# Group` heading, with a link to their Github homepage
1. When you commit your work, use the commit message to `close #` the ticket
1. Each member should create a pull request
1. As a group, sit together and select one person to merge all of the requests into `master`
1. After managing all merge conflicts, commit all the changes to `master` and push the branch to remote
1. Prune all of the name branches to demonstrate that functionality
1. On Slack, create a group message that includes all members of your group and the instructor, then paste the link to your Github Organization into it

## Project requirements

- Delegate roles to all group members
- Decide on any dependencies your team may wish to incorporate (ie, Sass, etc)
- Develop a plan for the layout of each page
- Decide on the general design system (colours, fonts, etc)
- Build a router that will navigate to all pages as an SPA
- All work must be done in branches
- All communication must go through "Issues", including (but not limited to):
  - Code bugs
  - Design decisions
  - Assigned tasks
  - Content changes
- Issues must be managed (open/comment/close)
- Include documentation (PDFs, compressed images, etc - no originals are necessary)

## Student data

Student data must be dynamic. Create one student template that accounts for all the possible information a student might share, but the information itself will be driven by stored data.

Although the ultimate goal would be to pull the data from a database/endpoint, start by using a local JavaScript `Array()`, fetching a local `.json` file, or working within `localstorage`, to ensure data can be loaded into the front-end without committing all the work to the backend. This will help you determine the fields necessary to complete the interface, before translating that to a formal data structure.

Student data should be determined by the url bar (location) and managed by your JS router. So for example, the url `location.pathname` might be set to `/student/tim-berners-lee` and thus would load information for a student name Tim Berners-Lee. Likewise, `/student/grace-hopper` would load data for Grace Hopper. However, both student pages are reading the same HTML template file, just populating the information from each student record independently based on the provided url scheme (sometimes called a "slug").

## Git management criteria

- Ensure each feature has its own branch during development _(don't use named user branches for all of your work!)_
- There should not be any `node_modules` folders in any of your branches
- Use `Issues` to track everything! Even if they're just upcoming features or proposals (use _labels_ to track their status/significance)
- All users should contribute to the Issues and documentation. Be sure to add a paragraph of text in the `README.md` file to explain your project and repository management strategy (how work was delegated, how pull requests and merges were handled, etc)

## Deliverables & Grades

The entire project is worth 25% of your final grade in WDDM-122.

### Part 1 (50% of grade)

Due: **Sunday, March 1 (before 11:59pm)**

Incorporated into each criteria are the the skills which should now be considered part of your workflow, including: syntax, spelling, documentation, code formatting, accessibility, efficient css rules, etc.

| Grade | Value | Description |
| --- | :---: | --- |
| Organization / Communication | 10 | Slack (or other) communication, issues/tickets, distribution of work, project management |
| Repository Management | 5 | Commit messages, branch names and usage, frequency of commits, fair distribution of work, file structure |
| SPA Framework (and other JS) | 5 | Usage and adjustments made to the "framework" structure to accommodate requirements |
| Content & Design | 15 | Development of assets, graphics, design prototypes, content, information architecture |
| Static Layout & Design | 15 | Prototyping pages using HTML/CSS |

### Part 2 (50% of grade)

Due: **Sunday, March 8 (before 11:59pm)**

Pages built with dynamic content and functionality.

| Grade | Value | Description |
| --- | :---: | --- |
| Organization / Communication | 10 | Slack (or other) communication, issues/tickets, distribution of work, project management |
| Repository Management | 10 | Commit messages, branch names and usage, frequency of commits, fair distribution of work, file structure |
| Static Layout & Design | 5 | Prototyping pages using HTML/CSS |
| Implementation | 25 | Development and implementation of functionality with Javascript, including dynamically loading student data into a single template. May include changes made to the SPA "framework" as well  |
