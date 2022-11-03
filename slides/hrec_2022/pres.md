# Data Storage Implications for Third Party Services

Aidan Wilson
Aidan.Wilson@acu.edu.au

Notes: I'm Aidan and I'm the Digital Research Analyst here at ACU, which means that I work between ORS and IT, helping them understand each other, and I also work with researchers when they need help or support with technology. Data storage is something I help out with quite a lot, and we in the eResearch team offer advice to researchers when they need to store data in particular places, encouraging them to use more university-standardised locations and services where appropriate, or thinking through some edge cases, such as when those researchers are collaborating with others outside the university. So it is in that context that I'm going to talk about data storage implications for third party services, and I'll speak specifically about Zoom, because it's a bit complicated here, but the general principles can apply to other sorts of services.

---

## Outline

- What is 'third party'?
- What's the problem?
- Data Storage
- Recordings
- Transcriptions
- General Guidelines

Notes: I'll talk about what I mean by third party, because it can mean different things to different people. Then I'll raise the main problem that we're trying to solve here, before I go into some areas that are impacted by this, namely, storage of data, of recordings, and transcriptions, both of which are related. Finally I'll raise some general guidelines.

---

## Third Party

"A third person or organization less directly involved in a matter than the main people or organizations that are involved" - Cambridge Dictionary<!-- .element: class="fragment" -->

"Third party is also used to refer to outsourcing certain functions to an outside company to ensure efficient service for clients." - Investopedia<!-- .element: class="fragment" -->

Notes: Third party obviously has a legal definition, which is this definition from Cambridge, but the specific meaning I'm using is this one by Investopedia. So the first two parties are ACU as a whole, and the researcher. Third party services therefore refers to any service that is utilised by the researcher but which is not provided by the university.

+++

### Storage:

|Not Third Party | Third Party |
|---|---|
|Network Drives|CloudStor |
| |OneDrive|
| |Dropbox|
| |Google Drive|

Notes: The fact that I have put some university approved services in the Third Party column, including CloudStor and OneDrive, when some might see these as being provided by the university. On a strict definition though, even though ACU may pay AARNet or Microsoft for their services, you could argue they are third party because they are not managed by the university. Perhaps there's cause for a third column here.

+++

### Data Collection

|Not Third Party | Third Party |
|---|---|
|REDCap|Qualtrics |
| |Survey Monkey|
| |LimeSurvey|
| |Google Forms|

+++

### Recording

|Not Third Party | Third Party |
|---|---|
| |Zoom |
| |Teams|
| |Google Meet|
| |Mobile apps|

---

## What's the problem?



Notes: The problem with using any third party service is that the university, and the researcher, cannot control what happens with that data, and usually what happens to it is hard to determine, even if you read the terms of service. 
There is risk with any third party service that the information you provide is no longer controlled by you or the university. This risk might be low, but the impact could be huge in the case of research data, so it is important for researchers to understand what's happening with their data.
There is an additional risk that some service that researchers have come to rely on changes without notice, or even ceases completely, leaving researchers stuck without a service, and the university caught in a tough position of having to find something to bridge the gap.

---

## Data Storage

- Shared drives (local)<!-- .element: class="fragment" -->
- CloudStor (AARNet)<!-- .element: class="fragment" -->
- OneDrive (Microsoft)<!-- .element: class="fragment" -->

Notes: Data storage is currently a bit of an issue at ACU. We're in the process of starting conversations around data storage with IT, but in a nutshell, the university right now cannot provide adequate storage infrastructure for projects that aim to capture a lot of data. With that in mind, the solution provided by the university is the local network drive system, shared drives, Isilon, Cohesity, whatever name you know it as. These are the drives that present to you as the R drive or the H drive on your computer.
There are two supported third party storage platforms that we use here, and they are CloudStor, operated by AARNet, the non-profit organisation that provides internet to Australian research institutions,
and OneDrive, operated by Microsoft as a huge, public, commercial cloud offering that we get as part of our subscription to things like Office365.

+++

### CloudStor

- 1TB free per individual account<!-- .element: class="fragment" -->
- 10TB free for group allocations<!-- .element: class="fragment" -->
- Provided through subscription to AARNet services<!-- .element: class="fragment" -->
- Shuttering in December 2023<!-- .element: class="fragment" -->

Notes: The university has never really provided much in terms of research data storage, and as a result we have, for some years now, been recommending people to use CloudStor as a stop-gap measure, since every account is allocated 1TB for no additional cost to the university, and with the potential to allocate higher volumes up to a total quota of 10TB that we get from AARNet for free.
CloudStor is provided to ACU as part of ACU's subscription to AARNet services, which are mainly things like IT network solutions, and access to the non-public, AARNet network.
The biggest problem with CloudStor though, is that they have as recently as two weeks ago announced that they are closing the service and deleting data in December 2023. This is certainly going to cause numerous headaches in the new year, and one solution, as problematic as it is, might be to ask researchers to move all their active data storage to:

+++

### OneDrive

- 1TB free for individuals<!-- .element: class="fragment" -->
- ?? group allocations<!-- .element: class="fragment" -->
- Provided through subscription to Office365<!-- .element: class="fragment" -->
- Not suitable for long-term storage<!-- .element: class="fragment" -->

Notes: In more recent years, we have begun recommending Microsoft OneDrive for storing research data, even sensitive data. We are not alone here; many other universities, including UNSW, Deakin, La Trobe and Sydney, are in the process of recommending OneDrive over all other options, and for all data classifications.
As a service it is very similar to CloudStor; individuals get 1TB of space that they can use, adequate for 90% of researchers, but whether larger volumes is possible with OneDrive I am unsure about.
It is provided by Microsoft to us as part of our subscription to Office365.
But there is a definite cloud, pardon the pun, over OneDrive as it is not suitable for long term storage. The reason for this is that OneDrive is tied to your Microsoft account. If that account ceases to exist, say, if you are an HDR student and you graduate, or if you are a staff researcher and you leave the university, your OneDrive data is deleted after a period that is determined by the tenant, in our case, by IT. I don't know what this period is for us, but it can only be between 30 days and 3650 days, so, one month to ten years, and that retention period cannot be differentially applied to research data or other kinds of data.
So we in eResearch are quite happy for people to use OneDrive for active data storage, but we have to begin putting pressure on researchers to clean up their data upon completion of their projects and put things in the right places, such as our digital repository, ResearchBank, though it is not capable of storing large volumes of data..

---

## Recordings

Notes: I'll leave the can of worms that is data storage and talk a little about recordings. It is a common use case here, particularly since COVID, that researchers will conduct interviews with research participants via phone or video meeting, and of course they will want to record those interviews so they can, for example, transcribe them and import the transcript into NVivo. After some 

---

## Transcriptions

---

## General Guidelines



