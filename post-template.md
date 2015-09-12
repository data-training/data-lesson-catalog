---
layout: page
permalink: /submit/
---

###Naming Conventions

Please name your file starting with a date in the format `Year-Month-Day` followed by a dash `-` and then a brief text description.

* Example: `2015-09-13-NEON-RLessons`
* We suggest the date you submit the document.


###Working with YAML

An example `YAML` header is below. Please note that the YAML starts and ends with `---`.
Comments are not supported.


	---
	layout: post
	catalog-entry-type: lesson               
	title: Lesson 01: Why Data Management
	description: Trends in data collection, storage and loss, the importance and benefits of data management, and an introduction to the data life cycle.
	authors: "Heather Henkel, Viv Hutchison, Carly Strasser, Stacy Rebich Hespanha, Kristin Vanderbilt, Lynda Wayne, Stephanie Hampton"  <<- open text unless we can automate this to create the YML files
	organization: [ DataONE, USGS ] 
	identifier: doi:xx.xxxx/example.doi
	license-name:                  
	target-audience:
	delivery-mode: 
	date-published: 2015
	citation: DataONE Education Module: Data Entry and Manipulation. DataONE. Retrieved Nov12, 2012. From https://www.dataone.org/sites/all/documents/L01_DataManagement.pptx
	topic-tag: ["Data Management and Processing", "Collaboration, Communication, and Dissemination"]              ---> from controlled vocab on topic taxonomy
	learning-type-tag: [Video, MOOC, In-Person, Podcast, Flipped Classroom, Powerpoint Slides, Powerpoint Slides with Video, Materials-based Exercise, blogpost]
	assessment-tag: 
	content-tag: 
	incentive-tag:  
	format-tag: 
	discrete-skills-tag:   
	software-language-tag: 
	time: 
	related-libraries: 
	source-url: https://www.dataone.org/education-modules
	image:  
	  feature: 
	  credit: 
	permalink: 
	comments: TRUE  
	event-coordinates: 
	event-location: the
	pre-req:
	---

---

###layout 

This tells jekyll how to render the past. Please use `post`

###catalog-entry-type: 
Select one of the following below unless your element fits into more than one. If it does, please let us know
so we can further consider design.

	catalog-entry-type: lesson

Use the controlled vocab: 

* lesson 
* data 
* unit 
* workshop 
* course 
* program 
* event

###title
This is the title of the element that you are submitting.

	title: "Lesson 01: Why Data Management"

###description
This is the description of the element that you are submitting. Please put your description in QUOTES.

	description: "Trends in data collection, storage and loss, the importance and benefits of data management, and an introduction to the data life cycle."

###authors
We need to decide whether to place authors in a jekyll parsable format or not. We probably should make it parsable??

	authors: "Heather Henkel, Viv Hutchison, Carly Strasser, Stacy Rebich Hespanha, Kristin Vanderbilt, Lynda Wayne, Stephanie Hampton" 

###organization
Please place the organization into a parsable list as following:

	organization: [ "DataONE", "USGS" ] 

###identifier
If your resource has a do, please place that here.

	identifier: doi:xx.xxxx/example.doi

###license-name
If you have a creative commons (or other license) associated with this, please add it here

	license-name: CC-BY 

###target-audience
We need to figure out how we want to group the target audiences. We could look at the taxonomy that other groups use.
  
	target-audience:

###delivery-mode
This describes how the content is delivered. It may be a video, a combination of text/graphics or an audio element. Are there others?

	delivery-mode:  video

###date-published
What year and month was the resource published?

	date-published: 2015

###citation 
Please place the text that users should use to cite the resource here.

	citation: DataONE Education Module: Data Entry and Manipulation. DataONE. Retrieved Nov12, 2012. From https://www.dataone.org/sites/all/documents/L01_DataManagement.pptx

###topic-tag
This is the skill set taxonomy list that we developed. Please use any of the controlled 
vocabulary words below to describe the content of your materials. Please any of the 6 
categories in square brackets separated by commas. There are 6 categories to select from.

Format: Square brackets with comma separated terms. You do not need quotes.

	topic-tag: [management-processing, collaboration-dissemination, communication-dissemination, analysis]              

* collaboration-synthesis 
* communication-dissemination
* analysis
* visualization
* management-processing
* software-skills
  
[To view the YAML list with slugs and easy to read names, please click here.](https://github.com/lwasser/data-lesson-catalog/blob/gh-pages/_data/topic-tags.yml)

[View the full skills taxonomy under development.](https://github.com/NCEAS/ds-workshop-2015/blob/master/skills-taxonomy.md)

#learning-type-tag
This tag seems to be a bit redundant with the format but also not very clear as to the goal of it.

	learning-type-tag: [Video, MOOC, In-Person, Podcast, Flipped Classroom, Powerpoint Slides, Powerpoint Slides with Video, Materials-based Exercise, blogpost]

###assessment-tag
i am not sure what this tag is either.
	assessment-tag: 

###content-tag
I am not sure what this tag is either.

	content-tag:                 

* Follows structure from Table 1. Knowledge and skills needed  

###incentive-tag
Is there any incentive to complete this resource? Some sort of credit? Please select from the list of
controlled vocal below.

	incentive-tag:  "University Credit"              
	
* badge
* UniversityCredit
* Certificate
* Open Access/No Credit   * i don't understand open access / no credit. can we just say no credit? *

###format-tag	
Please describe the format of the element using the list below. A workshop falls under `instructor lead lessons`. An online MOOC falls into `facilitated lessons`.

	format-tag: self-guided lesson                    

* self-guided lesson
* blog post
* facilitate lesson(s)
* instructor-lead lessons

###discrete-skills-tag
Matt - jekyll has tags and categories built in. this might be a good place to use the tags element as the list could get long over time. just a thought.

	discrete-skills-tag: [scripting, for-loops, statistical analysis, algorithm development]
	
We will build our list of skills over time. This should be automated to create the jekyll files needed to use tagging. We should start with a controlled list and ask users to add to it via some sort of "other" option if we build a form.

* scripting
* algorithm development
* for-loops
* statistical analysis

###software-language-tag

	software-language-tag:   R                 

* MatLab
* R
* Python
* SQL
*  

###time
The is the time that it might take to complete the lesson, workshop or course. 

	time:   "x hours"

Example options might include:

* 5 hours
* 1 week
* 2 weeks
* semester

###related-libraries

related-libraries:   <<- EG ggplot, matplotlib, etc

###source-url
This is the url that will take the user to the actual event homepage, lesson, etc.
	
	source-url: https://www.dataone.org/education-modules

###image
This is a branding feature. We will add specifications about the size of the image. It is a banner as designed now. 

`feature` is the path to the image banner. 
`credit` is a text string that allows you to add text below the banner.

image:   
  feature: 
  credit: NEON Education, Boulder - Colorado  

###permalink
This is the short URL that can be used to access the resource that you are submitting in the catalog.
**how should we handle this?? we might want to assign this automatically??**

	permalink: /NEON/R-lessons
	
###comments
Please set comments to true. This is how we will allow the community to respond to our lessons.

	comments: TRUE 

###event-coordinates
If you know the coordinate location of the event (in lat, long), please add it here!

	event-coordinates:   latitude, longitude

###event-location
Please add the city, state or city, country location here.

	event-location:  Santa Barbara, California
	
#pre-req
i am not sure how we are handling this and what we expect users to input here.

	pre-req:
Please end the front matter with `---`

	---

Any text that you add BELOW the three dashes will appear as content on the page. Feel free to add descriptive text about the lesson or event as you see fit. 