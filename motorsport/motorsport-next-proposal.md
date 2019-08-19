background-image: url(motorsport/img/bg-certus-slide.jpg)
class: background, center, middle

# MOTORSPORT next
# Web/Mobile Hybrid Proposal
.small.center[Author: Jonathan Visser   |   Version: final v1.0]
.logo[<img src="motorsport/img/logo.png"/>]

.customer-logo-dark[<img src="motorsport/img-motorsport-next-proposal/ms-logo.png"/>]

---
layout: true
<div id="footer-content"><p><strong>Fresh Ideas.</strong> Exceptional Outcomes.</p></div>
---


#### CONTENTS

.box[

* Objective
* Introduction
* Solution Context
* Current Solution Architecture
* Architectural Goals
* Solution Scope
* Solution Options
* Next Steps
* Next Step Investment
* The Way Forward
]

---

class:  red, objectives

# Objectives

* Open up the MotorSport "Possum" solution to streamlined and new web and mobile capabilities.
* Establish a pathway to a new, open, agile and adaptive technology stack.
* Enable more opportunities to strengthen brand and improve commercialisation and revenue generating activities. 

---

# Introduction

This presentation outlines the current and future states, sets some high-level goals and some related technology options to agree, and suggests some next steps.





---

.tight[
## Solution Context
]
.floatleft[Leveraging technology for business growth]
.floatleft[<img src="motorsport/img-motorsport-next-proposal/solution-context.png" width="100%"/>]

---

.tight[
## Current Solution Architecture
]

.floatright[<img src="motorsport/img-motorsport-next-proposal/current-architecture.png" width="340px"/>]
.sm-all[
* **WordPress:** 
	* internet portal
	* web content management
	* integrates event calendar data
* **AVIARC:**
	* bus. process/bus. logic
	* forms/data capture
	* content management
	* reporting
	* user identity and access
* **Postgres:**
	* data storage
]

---

# Architectural Goals

* Increase user adoption and satisfaction by delivering a superior web and mobile experience.
* Address technical debt whilst leveraging the existing good work and investment.
* Deliver a solution simple to extend and cost-effective to maintain.
* Leverage widely supported and portable technology to ensure long-term viability.

---


# Solution Scope
Limiting the immediate focus to the Event Registration use case:
.grid.x3[
.left.box.small.green.component[
** STREAMLINED EVENT REGISTRATION **
* View calendar
* Event form
* Payment form

** extensions **
* Add vehicle
* Add driver
* Update profile
]
.right.box.small.blue.component.tech[
** TECHNOLOGY** <br><br>
* Front-end framework
* Integration strategy
]
.right.box.small.yellow.inverse.questions[
** Questions **
* Limit to happy path for MVP?
* Any rentals other than transponders?
* Events ask for checking of profile details - include?
* Include up-sell offerings during payment?
* Improve calendar->event reg. (entry point) experience?
* MVP: event registration only?
]
]

---

.tight[
## Solution Options - UI
.floatleft[Front-end framework]
]
.small[
There are two main options to consider to deliver a smooth and modern user experience for desktop, tablet & mobile. Both move away from pure AVIARC approach; both require bespoke development.
]
.grid.small[.x[
#### WordPress Plugin/Widget
WordPress is a mature, widely used, and open platform with many existing extensions. It is currently being used to server the main website - which is "responsive" (works ok on mobile devices). It can be extended with custom components.
.closer[
###### Pros:
]
* Consolidates all front-end development onto a single platform.
* Seamlessly integrates with existing website.
* Supports CRM and e-commerce extensions.

.closer[
###### Cons:
]
* Originally for blogging.
* There are platform constraints and complexities to overcome.
* Cannot be used to replace Aviarc-embedded business logic.
]
.y[
#### Stand-alone modern bespoke Web App
With a variety of good options to chose from, open, flexible, with rapid development tooling, a bespoke responsive web application provides the best user-experience and future options.
.closer[
###### Pros:
]
* Light-weight, unencumbered, and fit for purpose.
* Opens architecture for improvements and scaling.
* Highly responsive/fast experience.

.closer[
###### Cons:
]
* Additional architectural layer - discrete from either AVIARC or WordPress.
]
] 

---


.tight[
## Solution Options - API
.floatleft[Integration strategy]
]
.small[
Possum contains complex business rules developed over time. This represents a very real challenge. There are distinct ways of dealing with this: wrap & reuse or rebuild clean. There are signficant strategic implications either way.
]
.grid.small[.x[
#### AVIARC API (wrap & reuse)
.closer[
###### Pros:
]
* Can leverage existing components such as databrokers/XMLCommands.
* Single codebase to maintain.
* Hides the complexity and defers dealing with it.

.closer[
###### Cons:
]
* Non-standard industry framework/toolsets that require heavy customisation and not following best practice.
* Hard to replicate full REST capabilities in Aviarc.
* Bound to Aviarc application/platform.
* Hard to test, hard to change.
]
.y[
#### Specialised API (rebuild clean)
.closer[
###### Pros:
]
* Industry standard frameworks/toolsets that are fit for purpose and can develop according to best practice.
* Can run independently of Aviarc application/platform - direct access to DB.
* Robust, secure and proven.
* Easily testable, easy to extend and maintain.

.closer[
###### Cons:
]
* Can’t leverage existing Aviarc components/business logic.
* Another codebase to maintain.
* Likely duplicate code - and potential for inconsistencies.
]
] 

---


# Next Steps

### Stage One - Planning and Design

.grid[.left.box.small.blue[ ** ARCHITECTURE & DESIGN **
* Requirements:
	* Wireframe/screen design
	* Requirements backlog
	* Out-of-scope items
	* Business logic documentation
* Architectural detailing:
	* Platform investigation & design
	* Integration scoping
]

.right.box.small.yellow[** PROJECT MANAGEMENT **
* Creation of a detailed implementation project plan:
  * Costings
  * Schedule
  * Resource plan
]]

---

.tight[
# Next Step Investment
]
.small[Because of the unknowns in scope, architecture, and business logic complexity, we recommend conducting a short discovery phase to enable planning.]
.tight[

### Discover: Planning & Design]

.small.condense[
| Activity          | Estimate Hours | Estimate Investment |
| ----------------- | -------------- | ------------------- |
| Requirements | .r[20] | .r[$3,300] |
| Architecture & Design| .r[24] | .r[$3,960] |
| Project Planning | .r[10] | .r[$1,650] |
| .r[**totals:**]	    | .r[**54 hrs**]	| .r[**NZ$8910**] |
* assumes scope is highly focused and doesn't spill out into related areas.

]

### Critical Success Factors

.tight.small[

* Decide on appropriate architectural strategy
* Agree on clear and focused first-version (MVP)  scope

]

---

class: center, blue

# The Way Forward

To take this proposal forward, we recommend the following three-stage approach:

1. **Planning and design:** Statement of Work, creation of formal requirements statement, architectural detailing, and creation of a detailed implementation project plan.
2. .decision[**Agree plan**]
3. **Implementation and go-live:** Statement of Work, including development, integration, software testing, and User Acceptance Testing support, and post-go-live production warranty.
