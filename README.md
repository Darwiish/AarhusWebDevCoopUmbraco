"# AarhusWebDevCoopUmbraco" 

Aarhus Web Developers Network – Umbraco Project
Description: Website for Aarhus Web Developers Network using Umbraco CMS and ASP.NET Core MVC.
---
---
Table of Contents

Introduction

Sitemap

Website Menu

Website Access Control

Contact Form

Conclusion

---
Introduction

This project focuses on building a website for the Aarhus Web Developers Network using Umbraco CMS.

Key technologies used:

Umbraco CMS – Open-source content management system

ASP.NET Core MVC – C# web application framework

Visual Studio – IDE for development

MS SQL Server – Database backend

The project demonstrates the creation of a functional website with structured navigation, access control, and user interaction through a contact form.

---
Sitemap

Created a Partial View to display the sitemap using a Site Map snippet.

A Sitemap Document Type was created with a corresponding template based on the Master template.

A document was added in the content tree to render the sitemap dynamically.

Sitemap generates a nested HTML list of visible pages using a custom Razor helper Traverse().

---

Website Menu

Developed a Master Document Type with common properties and SEO optimization.

Added umbracoNaviHide property to hide pages from the menu when needed.

Menu generation logic:

Select all visible children of the site root into an array.

Identify dropdown items with the alias projectsOverview.

Render the first five completed projects in descending order.

For each child, check visibility and access rights before rendering.

---

Website Access Control

Login System: Partial view loginForm + Login Document Type + Login Template.

Members: Created members in Umbraco backoffice to control access.

Login page added as a child of the Home node to manage authentication.

Restricted pages redirect unauthorized users to login.

---

Contact Form

Contact Document Type & Template created for form submission.

Model Class uses Data Annotations for server-side validation.

Controller:

Renders the form

Submits the data

Sends email notifications

Form rendered using a partial view, embedded in the Contact template.

---

Conclusion

Fully working website built on Umbraco CMS.

Flexible CMS but required time to fully understand and configure.

Content and functionality complete, with menu, sitemap, access control, and contact form fully operational.

Design could be improved with more time, but core functionalities work without errors.

Next Steps / Improvements:

Enhance front-end design and user experience.

Add analytics or reporting for member activity.

Expand member roles and access levels.
