# Doing a Shift

## Scheduling

- We use WhenIWork for scheduling (you should already have gotten an email about signing up). You can use this site to set your preferred hours and request time off.
- The schedule for learn experts is sent out every Wednesday for the following week. If you need any days off, book them *before* Wednesday the week before.
- As soon as you get your shifts, check them out and DM Avidor if they're not OK Wednesday night or Thursday morning
- Your shifts may get moved around Wednesday night/Thursday morning to accommodate others, but they should be fixed by noon on Thursday (all times ET)
- If the week is already schedule and something comes up where you need to swap a shift, please refer to the [How To Swap A Shift](https://github.com/flatiron-labs/learn-support/blob/master/how-to-swap-a-shift.md) doc in the learn-support repo. 

## Shift Types

There are two different types of shifts we are currently running:

- [One on one support shift](#one-on-one-support-shift) - One expert acts as dispatcher and takes in all incoming questions. They then hand out students that need support to do ~15min screen shares to the next available expert. 
- [Standard shift](#standard-shift) - All learn experts pick up questions as they come in and try and either help a few students at a time, or do screen shares when necessary. 

We do standard shifts on weekends (because we don't have enough people to do one on one) and one on one support on weekends. 


## Slack - Flatiron Staff

learn-experts channel: this is where we can ask questions and chat as a group. Use this channel in lieu of direct messages so we have a good sense of community and we can all learn from one another’s questions and answers.

escalation channel: You should not need to post directly into this channel. If you ever create an issue on Jira with a level of Blocking (more on this in later sections), it will automatically get posted here and you can watch any conversation around that. 

## One on one support

The one on one support model is based around giving each student a small but of your time, but all of your attention. We accomplish this by having one learn expert on the shift act as dispatcher and the rest providing the one on one support. 

- Go into Flatiron Staff Slack - #learn-experts
- Type `@here: in` to let people know you're on and ready for your shift
- Go to the [Learn Expert Chat](https://learn.co/expert-chat) window. It shows you all questions for the batches that we support. If a question is in expert chat, we support that batch.

### Dispatcher

If this is the first shift of the day, the experts on will have to decide between them who the dispatcher is. From there on out, the dispatcher is in charge of handing this roll off either sometime during their shift or at the end of their shift. 

One Learn Expert acts as Dispatch and logs all incoming chats here: https://docs.google.com/a/flatironschool.com/spreadsheets/d/13bueY7QZvfekgVwonlqfPCP8RdhMNK3BFoiJAl75QqM/edit?usp=sharing on the tab with today's date. The most important fields to mark down are in red (type, question_link, start_share, and end_share). If need be, all the other links can be filled in later (even though if it's a pain, please only skip them if it gets too busy). You can track the start and end times of each screen share by the learn experts saying `@here ss start` or `@here ss end` in Slack, and you won't know the type of question until a bit later.

The Learn Expert on dispatch greets all incoming chats and gets some preliminary information on them. 

If the issue is a simple question with a discrete answer (e.g. "What's the difference between `#find` and `#detect` in ruby?"), you can feel free to just answer it and/or direct them to a resource (e.g. "They're the same thing :) As you can see here: https://ruby-doc.org/core-2.2.3/Enumerable.html#method-i-detect they're used interchangeably."). Similarly, if the issue is solved by something in the Help Center, link them to the doc before linking the student to an expert.

If it's clear that the student will need more than a link and a few short answers, set them up with a screen share by saying something like:

>Thanks for clarifying the issue you're running into. Would now be a good time for you to screen share with a Learn Expert? Let me know, and also please make sure to already have TeamViewer 11 downloaded (https://www.teamviewer.com/en/download/previous-versions/) and your mic all set up :) If you already have Teamviewer installed, please make sure it is version 11.

Once the student lets you know that they're ready, ping the next available expert in Slack to pick up that student _or_ give the student an estimated wait time and connect an expert with them when one becomes available.

If it's getting busy, take a look at when experts _started_ their SS. If they've been on a share for 15 minutes already, start bugging them in slack and letting them know that they're coming up on time.

#### Filling out the spreadsheet

![question link](https://s3.amazonaws.com/learn-experts/question_link.png)

Getting the `question_link`. You can easily do this by right clicking here and selecting Copy Link Address and pasting it into the sheet.

A question link will look like this `https://learn.co/lessons/19011?batch_id=436&track_id=18316&question_id=44755`. Take a look at the last part there, `question_id=44755`, the `44755` is what get's filled into the `handraise_question_id` column in the spread sheet. 

Now, if you go to `learn.co/handraise_questions/44755` you'll easily be able to see that time that the question was asked at!

Question types:
 - SS - A screen share occurred
 - Not Supported - A question was asked on something that isn't supported (e.g. Assessments, python, algorithms)
 - Unable to SS - Cannot SS right now
 - Chat-Dispatch - Solved by dispatch quickly chatting with student and/or linking them off site
 - Chat-sync - Student handed off to rotation for a synchronous chat
 - No Answer - Student does not get back with anything actionable
 - Duplicate - Student already has a question on the same topic open

At the end of your shift, you are in charge of handing off this role to the next shift. Make sure some one is picking up as dispatch. Ask for a volunteer and hand it off to anyone who wants. Some minor etiquette on on handing off the dispatcher roll, please give anyone LE's who's on a double priority so that if they choose to break up their shift, they can. 

### The Screen Share

If you're not on Dispatch, then you'll be doing screen shares with students. If it's busy, please keep each session with a student to **20 minutes** (I'd recommend blocking out 15min for the screen share itself, and 5min for the setup time).

Please make sure to already be familiar with the [screen share doc](https://github.com/flatiron-labs/learn-support/blob/master/screen-sharing.md).

When you get assigned a screen share, make sure to say `@here ss start` and `@here ss finish` so the dispatcher can know when you started and finished your screen share.

Working within a time limit can be difficult and you won't be able to solve all problems in 15 minutes. That's OK. If you notice you're starting to come up on time, then try and leave off with the student in such a way that they have something that they can keep working on (e.g. "Try putting a `pry` here.", "Look into what the variable `index` equals in this method." "Take another look at this lesson on Rails Routes."...) and let them know if they still need a hand that they can hop back in the rotation for another screen share.

#### Student Cannot / Will Not Screen Share

If possible, let's try and find _some_ way to synchronously work with the student even if it's just video. We really want to make sure that we can give them some meaningful time where we give them our full attention to help them for those 15 minutes. 

## Standard Shift

- Go into Flatiron Staff Slack - #learn-experts
- Type `@here: in` to let people know you're on and ready for your shift
- Go to the [Learn Expert Chat](https://learn.co/expert-chat) window. It shows you all questions for the batches that we support. If a question is in expert chat, we support that batch.
- Optional: I would highly recommend installing [Nick's](https://github.com/NStephenson) Learn Expert [Chrome extension](https://chrome.google.com/webstore/detail/le3/hjjhpafjpkkjbdchnaeikofponobhngc). It allows you to track the messages that you're currently working on _and_ get better notifications when a question ends up in Requires Actions.
- Ask previous shift (if there was one) how things went and to post a list of threads they're in the middle of and want to hand over
- Introduce yourself on those threads and read the thread history so you're up to speed with the issue (let's not make students repeat themselves)
- You'll see there are three categories of questions - requires action, active questions and inactive questions:
  - **Requires Action** is any new question or any question where the student has responded and has been waiting > 15 mins for an expert response. These are top priority and we should keep it fairly empty. **If we see something in requires action, we want to move it out of there as fast as we can.**
  - **Active Questions** is for questions where an expert and a student are actively chatting.
  - **Inactive Questions** are questions where a student hasn't responded to an expert for at least 15 mins so you can ignore them until the student replies when they'll become active questions again.
- Respond to every active question on every thread that isn't being helped by another member of staff. If you can, help them all. If not, let them know you're busy but will try to get back to them as quickly as you can. We get that more than 1-3 lively threads at a time is challenging - just do what you can and enjoy the process!
- An active question is one where the OP (Original Poster) has made a comment that has not yet been responded to by a member of staff.
- If another student is genuinely being helpful to the OP, that's awesome. Encourage them and let everyone know you're there to help if they have problems/issues/questions.

## Ending a shift

- Welcome the people taking over your shift (if any) in the #learn-experts Slack channel.
- Post a list of all questions you're in the middle of with an update on each one.
- If there isn't an expert taking over from you, let everyone you're chatting with or have chatted with during the shift that you're going off shift. Let them know that the next person should be on (whenever they should be on).
- Please **fill out this [form](https://docs.google.com/a/flatironschool.com/forms/d/1lmIrLt4s3WFILxcNunUCXRwSNICfJWxQdTaDtUvizro/viewform)**.  Any time in the last half hour is good - don't stay late to do it, but make sure it gets done!
- Post `@here: out` into the learn-experts slack channel within Flatiron Staff
