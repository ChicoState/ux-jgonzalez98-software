# Easy Apply Isn't That Easy

I've been applying to SOC analyst roles for the past few weeks, and LinkedIn has become my main hunting ground. Most of my applications run through their "Easy Apply" button, which is supposed to let you apply to a job in seconds using the info already on your profile. That's the pitch. The reality is a little different.

## The Job Listing

I pulled up a SOC Analyst role at Trace3 and the page looked clean. Job title, location, how many people applied, and a big blue "Easy Apply" button. There was also a panel right above the button that told me my profile and resume "are missing some required qualifications." So before I even clicked anything, LinkedIn was telling me it had already read my resume and knew how I stacked up against the job.

<img width="687" height="725" alt="linkedln" src="https://github.com/user-attachments/assets/1816b14c-7519-4441-b3d0-973f3458d7c9" />


This is where **affordances** come in. An affordance is the visual cue that tells you what something does when you click it. The Easy Apply button is bright blue with the LinkedIn logo right inside it. It looks like a one click action. Combined with that match panel telling me LinkedIn already understood my background, the whole page set up the expectation that this was going to be fast.

## The Modal Opens

I clicked Easy Apply and a modal popped up. The first thing I noticed at the bottom was a small line that said "Application powered by Greenhouse." That was already weird. I clicked an Easy Apply button on LinkedIn, but the form behind it is actually a Greenhouse form embedded inside LinkedIn.

<img width="752" height="727" alt="image" src="https://github.com/user-attachments/assets/fcb40c01-ebeb-4eef-bdb7-34ecf3564c6d" />


This is where my **mental model** broke. A mental model is the picture in your head of how something should work based on what the product told you. The button said Easy Apply. The match panel said LinkedIn already knew my qualifications. I expected a fast, LinkedIn-native experience. Instead I was filling out a Greenhouse form that just happened to live inside a LinkedIn popup. From the user's side it should not matter who powers the backend, but it definitely matters when the experience doesn't match the promise the button made.

The next screen asked me to upload a resume, even though my resume was already on my LinkedIn profile. I picked one and kept going.

<img width="741" height="620" alt="image" src="https://github.com/user-attachments/assets/dacc9466-dda7-4a97-929a-c256003dde17" />


## The Redundancy Problem

Then I got to this screen, and this is the part that really got me.

<img width="750" height="725" alt="image" src="https://github.com/user-attachments/assets/75a0c0d5-7ca9-49aa-a141-a852441d4fef" />


The first field asks for my LinkedIn Profile. I am inside LinkedIn. I clicked Easy Apply on a LinkedIn job listing. My LinkedIn profile is the entire reason I am here. The form is asking me to manually paste a link to the exact site I am already using.

Then a little further down there is a question that says "How did you hear about this job?" with a list of checkboxes. The first option in the list is LinkedIn. I am applying to a LinkedIn job posting from inside the LinkedIn app and the form is asking me to confirm that I heard about it on LinkedIn.

This is a **recognition vs. recall** failure. Recognition vs. recall is the idea that good design should let users recognize information from what is already on screen instead of forcing them to recall or retype it. LinkedIn has my profile URL. LinkedIn knows I found the job on LinkedIn. The whole point of a connected system is that you do not have to keep re-telling it things it already knows. Instead the form treats me like I just walked in off the street with no history.

It is the kind of small thing that makes you stop and laugh, but it is also the moment where the "Easy" in Easy Apply stops feeling true.

## The Review

After a few more screens of questions, I got to the review page. Everything I had typed in was shown back to me with little "Edit" buttons next to each section.

<img width="753" height="725" alt="image" src="https://github.com/user-attachments/assets/bbb1e42f-bf95-4d32-a7f1-7bccbd55506e" />


The review page is actually one of the better parts of the flow. I could go back and fix anything without losing my progress. This is good **feedback**, which is the response a system gives so the user knows what happened. Up to this point the feedback in the modal had been pretty light, just a Next button and a progress bar ticking up. The review screen finally gave me a real sense of what I was about to submit.

But it also made the whole thing feel longer than the button promised. I had been told this was Easy Apply, and now I was on a full review page with 100 percent on the progress bar after filling out four screens of info that LinkedIn or my resume already contained.

## What LinkedIn Gets Right

To be fair, the modal itself is clean. The progress bar at the top is helpful because at least I know how far along I am. The review page lets me catch mistakes before I submit. And the match panel on the listing page is genuinely useful, because it gives me a heads up on whether I should even bother applying.

## What Could Be Better

The name should change. "Easy Apply" sets up an expectation the product cannot always meet, especially when the form behind it is a Greenhouse form asking for the same info LinkedIn already has. The fields that LinkedIn could fill in itself, like my profile URL or how I heard about the job, should be pre filled or hidden entirely. If LinkedIn already knows the answer, asking me to type it in is wasted effort on both sides. Easy Apply does not need to be reinvented. It just needs to stop asking me for things it already knows.
