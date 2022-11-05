## Data Storage Implications for Third Party Services

Aidan Wilson

Aidan.Wilson@acu.edu.au

Human Research Ethics Committee Retreat 2022

Notes: I'm Aidan and I'm the Digital Research Analyst here at ACU, which means that I work between ORS and IT, helping them understand each other, and I also work with researchers when they need help or support with technology. Data storage is something I help out with quite a lot, and we in the eResearch team offer advice to researchers when they need to store data in particular places, encouraging them to use more university-standardised locations and services where appropriate, or thinking through some edge cases, such as when those researchers are collaborating with others outside the university. So it is in that context that I'm going to talk about data storage implications for third party services, and I'll speak specifically about Zoom, because it's a bit complicated here, but the general principles can apply to other sorts of services.

---

## Outline

- What is 'third party'?
- What's the problem?
- Data Storage
- Recording interviews
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

|Local | Third Party |
|---|---|
|Network Drives|CloudStor |
| |OneDrive|
| |Dropbox|
| |Google Drive|

Notes: The fact that I have put some university approved services in the Third Party column, including CloudStor and OneDrive, when some might see these as being provided by the university. On a strict definition though, even though ACU may pay AARNet or Microsoft for their services, you could argue they are third party because they are not managed by the university. Perhaps there's cause for a third column here.

+++

### Data Collection

|Local | Third Party |
|---|---|
|REDCap|Qualtrics |
| |Survey Monkey|
| |LimeSurvey|
| |Google Forms|

+++

### Recording interviews

|Local | Third Party |
|---|---|
|Local device |Zoom |
| |Teams|
| |Google Meet|
| |Mobile apps|

---

## What's the problem?

- Little or no control over the data by ACU/Researcher<!-- .element: class="fragment" -->
- Third-party dictates terms<!-- .element: class="fragment" -->
- Service can change/cease without warning<!-- .element: class="fragment" -->

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

### Network Shares

- Limited space<!-- .element: class="fragment" -->
- Cannot be shared outside the university<!-- .element: class="fragment" -->
- Must be connected to VPN while off campus<!-- .element: class="fragment" -->
- Access control complex; request to IT<!-- .element: class="fragment" -->

Notes: The only 'local' option among data storage platforms is the network shared drives, these are the R: drive or H: drive or whatever.

Unfortunately the whole system is under a bit of strain at the moment and there's not a lot of space left. So requesting a large amount of space is likely to be refused. 

Network shares are only available to ACU users, and only while on campus or on the VPN, so this option is not particularly useful for collaborating with colleagues outside the university.

They're not particularly convenient for researchers to set up or use, and the fact that they use the organisation structure to assign shares, it can lead to cases in which some people have access to research data when they shouldn't. Access controls are handled via requests to IT, which brings a certain amount of administrative overhead, again limiting their use in this regard.

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

But there is a definite cloud over OneDrive as it is not suitable for long term storage. The reason for this is that OneDrive is tied to your Microsoft account. If that account ceases to exist, say, if you are an HDR student and you graduate, or if you are a staff researcher and you leave the university, your OneDrive data is deleted after a period that is determined by the tenant, in our case, by IT. I don't know what this period is for us, but it can only be between 30 days and 3650 days, so, one month to ten years, and that retention period cannot be differentially applied to research data or other kinds of data.

So we in eResearch are quite happy for people to use OneDrive for active data storage, but we have to begin putting pressure on researchers to clean up their data upon completion of their projects and put things in the right places, such as our digital repository, ResearchBank, though it is not capable of storing large volumes of data..

---

## Recording interviews

| Account type | Recording storage |
|---|---|
| Licensed | Zoom's public servers |
| On-Prem | CloudStor |

Notes: I'll leave the can of worms that is data storage and talk a little about recordings. It is a common use case here, particularly since COVID, that researchers will conduct interviews with research participants via phone or video meeting, and of course they will want to record those interviews so they can, for example, transcribe them and import the transcript into NVivo. When we in the eResearch team started getting queries from researchers about whether they could record in Zoom, we did some analysis, and found that:

+++

### Recording interviews: Zoom

| ACU user type | Zoom license |
|---|---|
| Staff | Licensed |
| Student | On-Prem |

Notes: So what kind of accounts do we have at ACU? Well, it depends, unfortunately, on whether you're staff or a student. Students are on-prem, meaning their recordings go to CloudStor, whereas staff are licensed, meaning their recordings go to Zoom's public cloud, wherever that is.

As a result we advised all users to only record Zoom meetings to their local computer, and then save them in CloudStor, OneDrive, or the network shares when the file is ready.

+++

### Recording interviews: Teams

- Domain separation between staff and students
- Recordings go to OneDrive in all cases
- No capacity for recording to local storage

Notes: When it comes to Teams, there are other things to be aware of. First of all, there is currently a hard separation between the student myacu domain and the staff acu domain for Microsoft services including Teams. This is being addressed, finally, but it means that Teams meetings set up by staff can present difficulties for students in accessing them, and vice versa.

Notwithstanding that, the recording aspect of Teams is a little cleaner. Recordings are saved to the user's OneDrive, and can be shared with others using the built-in OneDrive sharing features.

Teams doesn't have any option to record locally though, so if a researcher uses Teams for recording participant interviews, then that data is being stored on OneDrive, which may not always be ideal depending on the interviewees, the content, and so on.

---

## Transcriptions

| Platform and license | Transcription |
|---|---|
| Zoom (Licensed) | Yes, via Otter.ai |
| Zoom (On-prem) | No |
| Teams | Yes, via Microsoft? |


Notes: In almost all cases, researchers will want to transcribe their interviews, whether they've recorded them using Zoom, Teams, some other third-party app on their computer or mobile device, or a physical audio/video recording device.

Both Zoom and Teams offer built-in options for both closed captioning and automated transcripts, but, as you've probably guessed, it's complicated.

If you're a staff member, then your cloud-recorded Zoom meetings are automatically transcribed, and those transcripts can be downloaded from your Zoom account online. This is convenient, but the downside is that the service that performs the transcription is yet another third-party service called Otter.ai. This may be acceptable, but it puts additional pressure on the researcher, eResearch of the HREC to consider the terms of this third-party service.

If you're a student though, you don't have access to automatic transcription of your zoom meetings as a result of the fact that Cloud recordings are saved to CloudStor instead of to Zoom's public cloud. So with the additional security of being able to store cloud recordings on CloudStor, students lose the option to automatically transcribe their recordings.

Teams recordings are not automatically transcribed, but when a user is sent the link to the recording, they can click a button to have the audio transcribed by Microsoft's systems. It takes a little while to process, but once done, the time-coded transcript can be used to index through the file to go to exact points. I can't find any information about where the data goes in order to be transcribed though, so we don't know if Microsoft is using their own systems, or another third-party, and we don't know where the data is sent.

+++

## Transcription

Other options:
- Use OneDrive to transcribe files (video only)
- Use local computer's dictate feature to transcribe (Safest)
- Use Microsoft Online to upload a file to transcribe it into the Word document

Notes: There are other ways to transcribe recordings.

You can take advantage of whatever Microsoft is doing, and upload a video file to OneDrive, go to play it, and click 'generate transcript'. This is probably the best option because the transcript is time-coded and able to be downloaded as a .vtt file, which is a text based format that can be used, probably, in a variety of platforms (though, regrettably, NVivo does not seem to understand this format).

Another option, a safer one, is to use your computer's dictation feature that comes built in on recent versions of Mac and Windows computers. I tried this with my Mac, and even with no internet connection, the dictation feature worked well. I would advise this for transcribing sensitive material as you can be assured that the data is not leaving the computer. You can't, as far as I can tell, transcribe a file using this method, but you can listen to the file in your earphones and repeat it into the dictate function. This is a great method if your audio is perhaps not very clear, in which case automatic transcription wouldn't do so well, whereas you can repeat unclear sections into the dictate feature more clearly.

The last option I'll cover here is to use Microsoft Word online (this doesn't work using the local application), and select 'transcribe' under the 'dictate' options, and upload a file. The advantage of this is that Microsoft Word separates the transcript into different speakers, but it cannot be downloaded as a .vtt file, it can only be pasted into the Word document.

---

## General Guidelines


---

## Data Classification

| Platform | Highly Sensitive | Sensitive | Private | Public |
|---|---|---|---|---|
| Network | ✅ | ✅ | ✅ | ✅ |
| OneDrive | ❌ | ✅ | ✅ | ✅ |
| CloudStor | ❌ | ✅ | ✅ | ✅ |
| Computer | ❌ | ❌ | ✅ | ✅ |
| Dropbox | ❌ | ❌ | ❌|✅|

Notes: Just to let you know that we in eResearch are working on clarifying some of these issues so that researchers and HREC can make more informed decisions about various kinds of data. 

One such piece of work is to define a research data classification, a document that describes different kinds of data and how sensitive they are based on whether it is identifiable or not, whether it contains medical or health information, and what groups of people are represented in the data.

We will also provide guidance on the sorts of platforms may be used to store data of different classifications.

Knowing what we do about third party services like Zoom and Teams when it comes to recording meetings and transcribing them, this kind of documentation will hopefully make decision-making in this area much simpler, and hopefully will allow researchers to choose the right platform or method, rather than be directed by the Research Office.

