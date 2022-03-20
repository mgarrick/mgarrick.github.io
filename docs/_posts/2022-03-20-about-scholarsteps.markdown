---
layout: post
title:  "About ScholarSteps"
date:   2022-03-20 06:50:00 -0700
categories: scholarsteps
---
ScholarSteps has come a long way.

After six years of *pajama-driven development*[^pajama-driven-development], we now have a small development team preparing to launch ScholarSteps at UC Irvine.

[^pajama-driven-development]: Pajama-driven development: development of a hobby/side project done early in the morning or late at night, often while the programmer is wearing pajamas.

# What is ScholarSteps?

> ScholarSteps is software for managing the faculty merit and promotion process.  The application combines workflow, document management, enterprise access control, and forms to turn complex university policies and procedures into simple step-by-step flows.

# What is *faculty merit and promotion*?

> The merit and promotion process is an important tool for universities in retaining and advancing their faculty.  It governs salary increases, step increases, job title changes, and tenure for academic personnel.  Most large universities now use software to shepherd faculty review cases through dozens of steps across multiple levels of their organization.

Since 2010 UC Irvine has used software for merit and promotion, and while the software works well, support for it will end in 2023.  ScholarSteps will launch in July 2022 as a pilot to replace this software.

# The decision to pilot at UC Irvine

About a year ago I demo'd ScholarSteps for UC Irvine leadership.  I prepared by adding a "UCI-lite" workflow to ScholarSteps to illustrate how UCI's process could work under the software.  The demo went well and we later agreed to move forward with a pilot.  We would build out a small project team of three developers, a part-time QA engineer, our Academic Personnel partners, and myself.  We'd also provide staffing for the long-term support and maintenance of the system.

Today we have all positions filled with the exception of a final Ruby on Rails Software Engineer position.  The team is quickly moving through the product backlog to keep the project on target to launch July 2022.  This is exceptional given that we aren't fully staffed yet and new features and changes are suggested weekly (adding to our backlog).

# Our progress

The team has built upon the core ScholarSteps functionality, enhancing the software and tailoring to UC Irvine's business process.

We **provisioned the software on UCI servers**, allowing the whole team to test changes.  Our partners in Academic Personnel are now exploring the test site and sharing great suggestions for improving the system.

Faculty review cases can now be **returned to a prior level** for changes.  This is particularly important for the dean and central offices as they ensure compliance with university policy.

We've further tailored the software to UCI's business process.  Faculty profiles now support searchable **UCPath employee IDs**.  We've added initial support for UCI's **salary scales** which help departments propose the right salary for their faculty.  We've added a **salary offscale component** when faculty teaching, research, or service merit a higher salary than the scale suggests.  More UCI terminology is making its way into the system, hopefully making the future software transition easier on our analysts.  Finally, we've fine-tuned access for each UCI role, confirming that the right people have access to the right information during the right step of the workflow.

The Council on Academic Personnel can now **enter their recommendation** and Vice Provost can enter their final action.  These steps track important details such as the recommended salary, step, and more.  The **PDF bundle** now reflects all recommendations and final actions, ensuring that it contains everything faculty and administrators need to review a case.

**Committee members can now be recused** when conflicts of interest arise.  Recusing is important when the person being reviewed has a spouse or family member sitting on the committee.

On the technical side we've upgraded the underlying framework (Ruby on Rails) in order to keep pace with technology and avoid security vulnerabilities.  We've built out a respectable automated test suite, which now tests every step of the workflow from department to Vice Provost.  Github Actions performs these tests with every code change and automatically launches new releases.

I look forward to sharing more about our progress in the months to come.
