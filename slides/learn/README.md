# LITIS

Learn @ Intersect Training Introduction Slides
Built by Aidan Wilson

## About

This repository holds introduction slide content to be presented using [Reveal.js](https://revealjs.com/). Content is sourced dynamically from html files based on query string parameters.

## Landing page

If the GitHub pages base for the slides is loaded without at least a course parameter, the user is directed to a landing page where they can select a course and a university from drop-down menus, and reload the fully populated slide-deck.

## Structure

Slide-decks have six sections:

1. Title slide
2. Acknowledgement of Country
3. Intersect introduction
4. University introduction
5. Course introduction
6. Closing

Sections 2, 3 and 6 are constant across all courses, though may be periodically updated to reflect changes, such as to the number of researchers trained, or members/eRAs joining and leaving.

Sections 1 and 5 are sourced dynamically from the `course` query string parameter. The title slide is a simple course title, and the course introduction contains the course-specific slides. If the `course` parameter in the URL is missing, or does not resolve to a known course (as determined by the `resources.js` file), then the Landing Page (`course_select.html`) is displayed instead.

Note that the course _material_ is managed elsewhere, typically its own GitHub repository with its own URL. The point of these slides is not to replace the course material, but to briefly introduce the course. As such the materials in these slides might be very brief, and might consist of a broad overview of objectives and outcomes, an agenda, and setting expectations for attendees.

Section 4 is sourced dynamically from the `uni` query string parameter. The contents will introduce attendees to the host uni's specific information relating to Intersect and eResearch. It should contain the image and contact details of the eRA, information about research support, local events such as Hacky Hour or Digital Drop-In Sessions, and perhaps locally relevant links to more information. It is the responsibility of the eRA to manage the university introduction slide contents.

If the `uni` parameter in the URL is missing, or does not resolve to a known university (as determined by the `resources.js` file), then the university introduction section is omitted from the slide. This may be the case for an Open course, or one delivered outside the membership.

## File Structure

This repository has the following structure:
```
.
├── index.html
├── public.html
├── course_select.html
├── resources.js
├── course_title
│   └── {course_code}.html
├── course_intro
│   └── {course_code}.html
├── intersect_common
│   ├── aoc.html
│   ├── intersect_closing.html
│   ├── intersect_intro.html
│   ├── img
│   │   └── {uni_code}.png
│   └── profile_images
│       └── {era}.png
└── uni_intro
    └── {uni_code}.html
```

The main `index.html` file sources the required slide elements from the other directories and initializes the Reveal.js framework, loading some plugins, such as slide notes. 

The `public.html` file sources only the requested course introduction, and initializes the Reveal.js framework, only this time it does not load additional plugins like the slide notes plugin. The purpose of this `public.html` file is that it displays _only_ the course intro and can be embedded on the Intersect website on the relevant course page.

The `course_select.html` file is loaded when the `index.html` file is loaded without any value for the `course` parameter, or where the `course` parameter does not resolve to a known course (as determined by the `resources.js` file). This presents a simple landing page in which the user can select a course and optionally a university, and then submit the form to reload the slides page with the correct parameters, and load a fully populated slide-deck.

## Maintenance

The following are the major reasons that slides might need to be updated:

- A new member joins Intersect
- Intersect develops a new course
- Personnel movements, like a new or departing eRA

Additionally, slides may need to be updated for ongoing changes, like the number of researchers trained, or for information about events.

### New Member

When a new member joins, the following changes must be made.

1. The member is added to `resources.js` with their uni code and their full name
2. A `{uni_code}.html` file is added to the `uni_intro` directory named for the new member's uni code, which contains information about the eRA, any local events, resources, and so on
3. A new member logo added to the `intersect_common/img` directory
4. The `intersect_common/intersect_intro.html` slide component updated to include the new member logo

### New Course

When a new course is developed, the following changes must be made.

1. The course is added to `resources.js` with its course code and title.
2. A `{course_code}.html` file is added to the `course_intro` directory, named for the new course's code, which contains the introductory course slide content
3. A `{course_code}.html` file is added to the `course_title` directory, names for the new course's code, which contains just the first slide; the course title, then "A course by Intersect Australia", and a background image sourced from an online location such as unsplash.

### Personnel Movements

When an eRA leaves, joins, or moves university, the affected `uni_intro/{uni_code}.html` files must be updated to reflect the changes.

### Routine Maintenance

Other routine maintenance might be needed when a uni commences running a hacky hour, or changes the time of their hacky hour, or else some other locally relevant information changes. If these changes are within the context of a single uni, the `uni_intro/{uni_code}.html` file should be updated by the eRA.

Lastly, changes and updates to the `intersect_common/intersect_intro.html` or `intersect_common/intersect_closing.html` files may be necessary periodically. For example, when advertising a new event such as ResBaz, or updating training numbers.

