# Doing a Shift

## Scheduling

- All times for scheduling are in EST time
- The week is scheduled from Sunday to Saturday
- We use WhenIWork for scheduling (you should already have gotten an email about signing up). You can use this site to set your preferred hours and request time off.
- The schedule for Technical Coaches is sent out every Sunday for the following week. If you need any days off, book them *before* Friday.
- As soon as you get your shifts, check them out and DM Ruth if they're not OK by Sunday night or Monday morning
- Your shifts may get moved around till Tuesday morning to accommodate others, but they should be fixed by EOD Tuesday
- If the week is already scheduled and something comes up where you need to swap a shift, please refer to the [How To Swap A Shift](https://github.com/flatiron-labs/learn-support/blob/master/how-to-swap-a-shift.md) doc in the learn-support repo. 

## Shift Types

There are two different types of shifts we are currently running:

- [Standard Shift](#standard-shift) - One coach acts as dispatcher and takes in all incoming questions. They then hand out students that need support to do 20 minute screen shares to the next available coach. 
- [Chat only shift](#chat-only-shift) - All Technical Coaches pick up questions as they come in and try and either help a few students at a time, or do screen shares when necessary. 

We do chat only shifts occasionally on holidays (because we don't have enough people to do one on one).

## Slack - Flatiron Staff

technical-coaches channel: this is where we can ask questions and chat as a group. Use this channel in lieu of direct messages so we have a good sense of community and we can all learn from one another’s questions and answers.

escalation channel: You should not need to post directly into this channel. If you ever create an issue on Jira with a level of Blocking (more on this in later sections), it will automatically get posted here and you can watch any conversation around that.

technical-coach-updates: This channel is used for viewing updates on any maintenance, bug fixes, ide updates, batch notices, etc... Do not chat in this channel as it is used only for viewing these changes.

## Helpful Resources
You might want to have these pages bookmarked for each shift:
- [expert chat](https://learn.co/expert-chat)
- [help docs](http://help.learn.co/)

optionally you can install Nick's Chrome Extension for Tracking Questions:
- [Chrome Extension](https://chrome.google.com/webstore/detail/le3/hjjhpafjpkkjbdchnaeikofponobhngc)

## Categories of questions

You'll see there are three categories of questions - requires action, active questions and inactive questions:
  - **Requires Action** is any new question or any question where the student has responded and has been waiting > 15 mins for a coach response. These are top priority and we should keep it fairly empty. **If we see something in requires action, we want to move it out of there as fast as we can.**
  - **Active Questions** is for questions where a coach and a student are actively chatting.
  - **Inactive Questions** are questions where a student hasn't responded to a coach for at least 15 mins so you can ignore them until the student replies when they'll become active questions again.

## Standard Shift

The one on one support model is based around giving each student a small bit of your time, but all of your attention. We accomplish this by having one Technical Coach on the shift act as dispatcher and the rest providing the one on one support. 

- Go into Flatiron Staff Slack - #technical-coaches
- Type `@qbot in <role>` to log into your shift. You can either log in as `sync` or `dispatch`. If you're just starting out, you'll do `sync` and as you learn, you can hop on dispatch. 
- Go to the [Expert Chat](https://learn.co/expert-chat) window. It shows you all questions for the batches that we support. If a question is in expert chat, we support that batch.

### Dispatcher

If this is the first shift of the day, the Coaches on will have to decide between them who the dispatcher is. You will then `qbot in dispatch` in the #technical-coaches channel. From there on out, the dispatcher is in charge of handing this roll off either sometime during their shift or at the end of their shift. 

The Technical Coach on dispatch greets all incoming chats and gets some preliminary information on them. 

- If the issue is a simple question with a discrete answer (e.g. "What's the difference between `#find` and `#detect` in ruby?"), you can feel free to just answer it and/or direct them to a resource (e.g. "They're the same thing :) As you can see here: https://ruby-doc.org/core-2.2.3/Enumerable.html#method-i-detect they're used interchangeably."). Similarly, if the issue is solved by something in the [Help Center](http://help.learn.co/), link them to the doc before linking the student to a coach.

- If it's clear that the student will need more than a link and a few short answers, set them up with a screen share by saying something like: 
```
"Would you like to have a 20 minute pair programming session with a technical coach via screen share?"
```
**Make sure to add 20 minute pair programming session when you ask the student if they want a screen share, this lets will get them used to the idea of pair programming with another developer**, this also lets them know that Technical Coaches are alloted 20 minutes per screen share.

- Once the student lets you know that that would work for them, copy the question link by clicking on the clipboard:

![question link](https://s3.amazonaws.com/learn-experts/expert-chat-clipboard.png)

- And pasting to the technical-coaches channel to queue up the question for the next available coach on sync support.

- You will also want to keep track of the screen shares that the sync's are currently on. You can type `qbot who is on?`, which will give you who has a question, how long they've been on a screen share, and who is free. Make sure to do this periodically. At 15-18 minutes, you can type something like: "`@username 15 minute mark!`" which will send a notification to them letting them know they only have 5 minutes left. If they are past the 18 minute mark, you would type something like: "`@username 18 minutes! Please wrap up!`". We try to be fair to our students and give them all the same amount of attention.

- If another student is genuinely being helpful to the OP, that's awesome. Encourage them and let everyone know you're there to help if they have problems/issues/questions.

- If you notice there are a lot of questions in expert chat, and the sync's are free of screen shares, make sure to keep them queue'd up. You can check the queue by typing `qbot q`. That way each student gets proper one on one support.

- If you queue a student and they have figured out the issue. You can `qbot resolve question_id`. You can find the question id by typing `qbot q` and you will see something like `https://learn.co//lessons/25366?batch_id=306&track_id=23144/&question_id=96994`. In this example you could type `qbot resolve 96994` in order to resolve the question. The question will then be resolved and removed from the queue.

At 5 minutes before your shift ends, make sure to type "`@here dispatch available in 5 minutes`", in order to let the coaches coming in know that dispatch will be available and someone can grab dispatch. Once your shift is over, type `qbot out` in order to end your shift and mark your hours in workday.

**Do not resolve questions for students, only resolve questions that the last respond time the original poster made was 10 hours or more**

### Sync Support

If you're not on Dispatch, then you'll be doing screen shares with students. Please keep each session with a student to **20 minutes** (I'd recommend blocking out 15min for the screen share itself, and 5min for the setup time). qBot will slack you when you have a chat. You can then start a Zoom meeting and send the student an invite link. Also when you say hi to them, you can @mention them when you introduce yourself. That way they get a notification if they have chat minimized, for example: "`Hey @enoch2k2! here's the link for our 20 minute screen share! https://zoom/2343252`" (not a real link).

Please make sure to already be familiar with the [screen share doc](https://github.com/flatiron-labs/learn-support/blob/master/screen-sharing.md).

Working within a time limit can be difficult and you won't be able to solve all problems in 15 minutes. That's OK. If you notice you're starting to come up on time, then try and leave off with the student in such a way that they have something that they can keep working on (e.g. "Try putting a `pry` here.", "Look into what the variable `index` equals in this method." "Take another look at this lesson on Rails Routes."...) and let them know if they still need a hand that they can hop back in the rotation for another screen share.

- If you feel the student needs more help, for example you were unable to find out what the issue was. Let the student know that you are out of time and would like a fresh pair of eyes to view their issue and ask them if you can place them back in the queue. Most students appreciate this and don't mind getting placed back in the queue. To place them back in the queue you can type `qbot more help` in the technical-coaches channel. Also let the student know after you added them back into queue that they were placed back in queue.

- If you feel the student has been resolved, you can resolve the question you have with `qbot done`. It's also nice to leave them with a farewell in chat after you wrap up in a screen share. Also you can remind them to resolve the chat.

- If you respond to a student with a link, and they do not reply to you in 5 minutes, you will want to mark them `unresponsive` by typing in `qbot unresponsive`, this will place the question on hold for 5 minutes before assigning the question to the next available technical coach. If you are the technical coach that gets assigned an `unresponsive` question. If they have still not replied since the last link was given. You can `qbot unresponsive`. If you notice the question was responded to greater than 30 minutes, then you can `qbot done` the question in order to resolve.

- If you have no screen share, you will need to go through the `inactive questions` and mark any questions with a response of 10 hours or older resolved. Make sure to type to them something like: `"Hello! It looks like this question has been inactive for over 10 hours and will be resolved. If you still need help please open a new question. We’ll be more than happy to help! Thanks!"`. They will recieve an email with that last response, so if they are looking for their chat, they know why it was resolved.

- If all the older inactive questions have been resolved and you still don't have a screen share. You will need to help the dispatch out. Pick a question to help out with, click the clipboard at the top as if you were going to queue up a question (see above image). Paste into technical-coaches chat, replace `queue` with `take`. The format should look like `qbot take <link>`. That will assign the question to you. Then you can help them in chat and ask if they would like a screen share.

Make sure to keep an eye on your times and in slack if the dispatch tells you that you are close to time. You can send a dm in Flatiron Staff to `qbot`. And type `qbot who is on?` in order to see how long you have been on a screen share. If you get to around 18 minutes. Make sure to wrap up with the student. If they still need help make sure to `qbot more help` and follow the guidelines described above.

At the end of your shift, if you recieve a question 5 minutes prior to the end of your shift, you can `qbot more help`. If you recieve a question 2 minutes prior to the end of your shift, you will need to `qbot more help` and then `qbot out`. Any questions assigned to you for 2 minutes or longer will need to be added back to the queue before you `qbot out`.

#### Student Cannot / Will Not Screen Share

If possible, let's try and find _some_ way to synchronously work with the student even if it's just video. We really want to make sure that we can give them some meaningful time where we give them our full attention to help them for those 15 minutes.

If they have bad internet, you can do chat only support (no screenshare). It's always a good idea to have them `learn save` in order to push up their code on github. Once they have pushed their code, you can get the url from clicking on:

![github link](https://s3.amazonaws.com/learn-experts/expert-chat-github-link.png)

This will take you to their forked repository and you can get the url to clone their repo. This will allow you to debug with the student and you can see all their errors locally.

## Chat Only Shift

We do the chat only shift on some holidays, if we don't have enough people to do one on one support.

- Go into Flatiron Staff Slack - #technical-Coaches
- Type `@qbot in sync` to let people know you're on and ready for your shift
- Go to the [Expert Chat](https://learn.co/expert-chat) window. It shows you all questions for the batches that we support. If a question is in coach chat, we support that batch.
- Ask previous shift (if there was one) how things went and to post a list of threads they're in the middle of and want to hand over
- Introduce yourself on those threads and read the thread history so you're up to speed with the issue (let's not make students repeat themselves)
- Respond to every active question on every thread that isn't being helped by another member of staff. If you can, help them all. If not, let them know you're busy but will try to get back to them as quickly as you can. We get that more than 1-3 lively threads at a time is challenging - just do what you can and enjoy the process!
- An active question is one where the OP (Original Poster) has made a comment that has not yet been responded to by a member of staff.

## Ending a shift

- Welcome the people taking over your shift (if any) in the #technical-coaches Slack channel.
- If there isn't a coach taking over from you, let everyone you're chatting with or have chatted with during the shift know that you're going off shift. Let them know that the next person should be on (whenever they should be on).
- Post `@qbot out` into the #technical-coaches slack channel within Flatiron Staff
- Please go on WorkDay and add your shift. 

##### Video Examples of Screen Share Sessions
- [example 1](https://youtu.be/8d07IoGX7UQ)
- [example 2](https://youtu.be/0Rege7kJoM8)
- [example 3](https://youtu.be/MURwX6jUlRk)
- [example 4](https://youtu.be/zzf-cd71-2U)
- [example 5](https://youtu.be/aMZFyDrT0S4)
- [example 6](https://youtu.be/oM1ge18NEZ8)
- [example 7](https://youtu.be/q2WoFBdyXxI)
- [example 8](https://youtu.be/FYsM3V5GMuE)
- [example 9](https://youtu.be/EIUB8CmpsFU)

<p class='util--hide'>View <a href='https://learn.co/lessons/learn-expert-doing-a-shift'>Doing a Shift</a> on Learn.co and start learning to code for free.</p>
