# Doing a Shift

## Scheduling

- All times for scheduling are in EST time.
- We use WhenIWork for scheduling (you should already have gotten an email about signing up). You can use this site to set your preferred hours and request time off.
- The schedule for Technical Coaches is sent out every Sunday for the following week. If you need any days off, book them *before* Friday.
- As soon as you get your shifts, check them out and DM Ruth if they're not OK by Sunday night or Monday morning
- Your shifts may get moved around till Tuesday morning to accommodate others, but they should be fixed by EOD Tuesday
- If the week is already scheduled and something comes up where you need to swap a shift, please refer to the [How To Swap A Shift](https://github.com/flatiron-labs/learn-support/blob/master/how-to-swap-a-shift.md) doc in the learn-support repo. 

## Shift Types

There are two different types of shifts we are currently running:

- [One on one support shift](#one-on-one-support) - One coach acts as dispatcher and takes in all incoming questions. They then hand out students that need support to do 20 minute screen shares to the next available coach. 
- [Standard shift](#standard-shift) - All Technical Coaches pick up questions as they come in and try and either help a few students at a time, or do screen shares when necessary. 

We do standard shifts occasionally on holidays (because we don't have enough people to do one on one).

## Slack - Flatiron Staff

technical-coaches channel: this is where we can ask questions and chat as a group. Use this channel in lieu of direct messages so we have a good sense of community and we can all learn from one another’s questions and answers.

escalation channel: You should not need to post directly into this channel. If you ever create an issue on Jira with a level of Blocking (more on this in later sections), it will automatically get posted here and you can watch any conversation around that.

technical-coach-updates: This channel is used for viewing updates on any maintenance, bug fixes, ide updates, batch notices, etc... Do not chat in this channel as it is used only for viewing these changes.

## One on one support

The one on one support model is based around giving each student a small bit of your time, but all of your attention. We accomplish this by having one Technical Coach on the shift act as dispatcher and the rest providing the one on one support. 

- Go into Flatiron Staff Slack - #technical-coaches
- Type `@qbot in <role>` to log into your shift. You can either log in as `sync` or `dispatch`. If you're just starting out, you'll do `sync` and as you learn, you can hop on dispatch. 
- Go to the [Expert Chat](https://learn.co/expert-chat) window. It shows you all questions for the batches that we support. If a question is in expert chat, we support that batch.

### Dispatcher

If this is the first shift of the day, the Coaches on will have to decide between them who the dispatcher is. You will then `qbot in dispatch` in the technical-coaches in slack. From there on out, the dispatcher is in charge of handing this roll off either sometime during their shift or at the end of their shift. 

The Technical Coach on dispatch greets all incoming chats and gets some preliminary information on them. 

If the issue is a simple question with a discrete answer (e.g. "What's the difference between `#find` and `#detect` in ruby?"), you can feel free to just answer it and/or direct them to a resource (e.g. "They're the same thing :) As you can see here: https://ruby-doc.org/core-2.2.3/Enumerable.html#method-i-detect they're used interchangeably."). Similarly, if the issue is solved by something in the [Help Center](http://help.learn.co/), link them to the doc before linking the student to an coach.

If it's clear that the student will need more than a link and a few short answers, set them up with a screen share by saying something like: "Would you be able to do a `20 minute screen share` with one of our other Technical Coaches? I think they could better help you with this through a screen share.". Make sure to add `20 minute screen share` when you ask the student if they want a screen share, this lets them know that Technical Coaches are alloted 20 minutes per screen share.

Once the student lets you know that that would work for them, copy the question link by clicking on the clipboard:

![question link](https://s3.amazonaws.com/learn-experts/expert-chat-clipboard.png)

And pasting to the technical-coaches channel to queue up the question for the next available coach on sync support.

You will also want to keep track of the screen shares that the sync's are currently on. You can type `qbot who is on?`, which will give you who has a question, how long they've been on a screen share, and who is free. At 15-18 minutes, you can type something like: `@username 15 minute mark!` which will send a notification to them letting them know they only have 5 minutes left. If they are past the 18 minute mark, you would type something like: `@username 18 minutes! Please wrap up!`. We try to be fair to our students and give them all the same amount of attention.

If you notice there are a lot of questions in expert chat, and the sync's are free of screen shares, make sure to keep them queue'd up. That way each student gets proper one on one support.

### Sync Support

If you're not on Dispatch, then you'll be doing screen shares with students. If it's busy, please keep each session with a student to **20 minutes** (I'd recommend blocking out 15min for the screen share itself, and 5min for the setup time). qBot will slack you when you have a chat. You can then start a Zoom meeting and send the student an invite link. 

Please make sure to already be familiar with the [screen share doc](https://github.com/flatiron-labs/learn-support/blob/master/screen-sharing.md).

Working within a time limit can be difficult and you won't be able to solve all problems in 15 minutes. That's OK. If you notice you're starting to come up on time, then try and leave off with the student in such a way that they have something that they can keep working on (e.g. "Try putting a `pry` here.", "Look into what the variable `index` equals in this method." "Take another look at this lesson on Rails Routes."...) and let them know if they still need a hand that they can hop back in the rotation for another screen share.

You can end a screen share by doing `@qbot done`, `@qbot unresponsive`, or `@qbot more help`. You can DM qBot `help` for more info on each command. 

#### Student Cannot / Will Not Screen Share

If possible, let's try and find _some_ way to synchronously work with the student even if it's just video. We really want to make sure that we can give them some meaningful time where we give them our full attention to help them for those 15 minutes. 

## Standard Shift

- Go into Flatiron Staff Slack - #learn-Coaches
- Type `@qbot in sync` to let people know you're on and ready for your shift
- Go to the [Technical Coach Chat](https://learn.co/coach-chat) window. It shows you all questions for the batches that we support. If a question is in coach chat, we support that batch.
- Optional: I would highly recommend installing [Nick's](https://github.com/NStephenson) Technical Coach [Chrome extension](https://chrome.google.com/webstore/detail/le3/hjjhpafjpkkjbdchnaeikofponobhngc). It allows you to track the messages that you're currently working on _and_ get better notifications when a question ends up in Requires Actions.
- Ask previous shift (if there was one) how things went and to post a list of threads they're in the middle of and want to hand over
- Introduce yourself on those threads and read the thread history so you're up to speed with the issue (let's not make students repeat themselves)
- You'll see there are three categories of questions - requires action, active questions and inactive questions:
  - **Requires Action** is any new question or any question where the student has responded and has been waiting > 15 mins for an coach response. These are top priority and we should keep it fairly empty. **If we see something in requires action, we want to move it out of there as fast as we can.**
  - **Active Questions** is for questions where an coach and a student are actively chatting.
  - **Inactive Questions** are questions where a student hasn't responded to an coach for at least 15 mins so you can ignore them until the student replies when they'll become active questions again.
- Respond to every active question on every thread that isn't being helped by another member of staff. If you can, help them all. If not, let them know you're busy but will try to get back to them as quickly as you can. We get that more than 1-3 lively threads at a time is challenging - just do what you can and enjoy the process!
- An active question is one where the OP (Original Poster) has made a comment that has not yet been responded to by a member of staff.
- If another student is genuinely being helpful to the OP, that's awesome. Encourage them and let everyone know you're there to help if they have problems/issues/questions.

## Ending a shift

- Welcome the people taking over your shift (if any) in the #learn-Coaches Slack channel.
- If there isn't an coach taking over from you, let everyone you're chatting with or have chatted with during the shift that you're going off shift. Let them know that the next person should be on (whenever they should be on).
- Post `@qbot out` into the learn-Coaches slack channel within Flatiron Staff
- Please go on WorkDay and add your shift. 

<p class='util--hide'>View <a href='https://learn.co/lessons/learn-coach-doing-a-shift'>Doing a Shift</a> on Learn.co and start learning to code for free.</p>
