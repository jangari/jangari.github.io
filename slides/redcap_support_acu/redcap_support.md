# REDCap Support at ACU

Aidan Wilson

Notes: I'm Aidan and I'm the main REDCap admin at ACU, and I'd like to talk about our support model.

---

## REDCap Support at ACU

- No dedicated REDCap personnel
- Little to no budget

Notes: Our support model at ACU is pretty thin. We are a team of two, Rod Lewis, who's day job is managing the research systems for the entire research office, which keeps him busy enough, and me, the eResearch Analyst from Intersect. REDCap adminstration, training and support is probably the majority of my job. Luckily, it's a tool I love.

---

## Intersect

- eResearch Services organisation
- Member since 2015
- Access to training
- Local eRA
- Data storage, cloud computing, HPC, engineering,

Notes: I should mention here that ACU is a member of Intersect Australia, a non-profit eResearch services organisation, which provides member universities with services including training, as well as a locally embedded resource, an eResearch Analyst, which is me.

---

## REDCap at ACU

- REDCap since 2016
- Huge growth in last couple of years
- Core part of ACU's research infrastructure
- Moderate interaction with Ethics
- Modest usage
	- 168 users (284 inactive/suspended)
	- 382 projects (161 production)

Notes: ACU has had REDCap since 2016 when it was installed at the request of a team of researchers from one of the high-performing institutes. Back then it was run by one person, my predecessor, who managed to get a modest VM from IT. I took over in about the middle of 2016, somewhat begrudgingly. Since then it has grown a lot, particularly since 2018 when we started offering training, and also started taking an active interest in researchers' use. Before this people could do what they wanted, and a couple of minor incidents forced our hand in, at first, requiring an admin to approve projects and the like. 

Now, REDCap is a core system at ACU, and it has strong support from research office and IT, and we have some interaction between Ethics and REDCap, particularly when it comes to eConsent, project approvals, and also since REDCap is simply the best way to manage sensitive, record level data.

We're still pretty small, with 168 active users, although lots of suspended users since we automatically suspend after 180 days) and 380 odd projects of which 161 are in production.

---

## Support and Training

Support:
- Consultation and advice by me
- Escalation to REDCap team within Intersect
- Escalation to Consortium Community

Training:
- Intersect courses
	- REDCAP101 (Beginner level)
	- REDCAP201 (Intermediate)
- 242 people trained in 19 courses

Notes: As it stands the support we offer for REDCap is simply me, perhaps assisted by my colleagues from Intersect; we have a group of eResearch Analysts who do lots of redcap support and admin for their unis, and we often help each other there. Also occasionally escalating to the Community where I can't help myself.

When it comes to training, ACU makes available technology training primarily via its membership of Intersect, and REDCap is no different. It's usually delivered by me but there is a team of people at Intersect working on the training from the administrative side, and a large team of trainers whom I often draw on to help manage the online zoom courses. So it's a team effort, and without Intersect, maybe I could run it myself, but I'm glad to not have to.

We run a basic intro course and a slightly more advanced course on longitudinal projects, and we're thinking of developing more advanced courses in future on topics like integrating with R, using the API, more advanced topics in survey design and so on.

We have trained 242 people in 19 courses in REDCap at ACU. I plan to move this into more of a BAU offering, say, quarterly. It would be good to require new users to take at least the intro course before they start building projects, but sometimes, the numbers are simply not there to justify a course. 

---

## Growth since COVID

- Increase in REDCap use since COVID
- More awareness of REDCap after engagement activities
- Explosion of (major) support requests

Notes: In the last couple of years, with both COVID, and a lot of engaging with researchers and research centres about REDCap, its use began to increase, and along with it, there was an explosion of support requests. Sometimes these requests were demanding a lot of our resources (read: my time).

---

### Usage Guidelines

<iframe width="800" height="500" data-src="https://rdcap.acu.edu.au/guidelines/#user-training-and-support" data-preload></iframe>

rdcap.acu.edu.au/guidelines/

Notes: To fix that, In May, we published some usage guidelines. These guidelines explain what users may do, who may get an account, what processes we go through in the project pipeline, i.e., no collecting real data unless you're in production mode, and that we check with ethics to see that your project is approved before we move it to production. And other business rules, policies and so on.

It also spells out what users can expect regarding support and training. In particular it puts a hard limit on us building projects for others. This gave us the means to say no to the more demanding users, and set expectations.

---

## Gaps, future plans

- Hacky hour / Digital drop-in session
- REDCap Users' group
- Extramural users' group?
	- redcap.stackexchange.com?
- Other ideas?

Notes: There are of course gaps. One big gap right now and something I'm planning on fixing as soon as this month is that we don't run a local hacky hour, data clinic, digital drop-in session, where researchers can bring their problems and speak to someone who might have the skills needed to help. REDCap would be just one technology that would be supported here, but I reckon it would feature heavily.

We also want to set up a REDCap users' group. We actually do have one, but we're using Microsoft Teams and the platform is simply not conducive to that sort of group. The activity in this group has been lacklustre. I'm hoping to broaden it to encompass all tools and have REDCap as one channel in the team.

Lastly, something I've been hoping to work on for a while but for which I've lacked the time and energy, is some sort of cross-institutional user support group for users to network and share ideas with others outside their organisation. There was a little appetite for this a couple of years ago and I suggested a redcap stackexchange, but we never quite got our act together and building a stackexchange actually takes quite a lot of work.

I would also be keen to hear others' thoughts on this because I suspect lots of us see many of the same kinds of support requests and they could easily be helped by peers without admins needing to get involved.

---

## Reach out

Aidan.Wilson@intersect.org.au

@aidan.wilson

Notes: So that's it from me. Reach out to me via email if you like, or in the community.

---

Here's a bit of code:

```json [2|3|4|5-9]
{
    "name": "HIDESUBMIT Action Tags",
    "namespace": "INTERSECT\\HideSubmit",
    "description": "Allows users to conditionally hide various Submit/Save/Next instance buttons on surveys and/or data entry forms using Action Tags and branching logic.",
    "permissions": [
        "redcap_survey_page_top",
        "redcap_data_entry_form_top",
        "redcap_every_page_before_render"
    ],
    "framework-version": 6,
    "authors": [
        {
            "name": "Aidan Wilson",
            "email": "aidan.wilson@intersect.org.au",
            "institution": "Intersect Australia"
        }
    ],
    "compatibility": {
        "redcap-version-min": "10.4.1"
    }
}
```
