## Jira Setup

This lab will cover installing Jira and integrating it with Slack and the Balerica Bank instance.

### jira_install.md completion
- [x] I created my own Atlassian account.
- [x] I can open my Jira Cloud site.
- [x] I selected or confirmed the Free plan.
- [x] I created the Balerica AI Incident Management project.
- [x] I know my actual project key.
- [x] I created and opened a manual test incident.
- [x] I saved the site URL, email, project key, and test issue key privately.
- [x] I have not shared any passwords or API tokens.

Despite all of the above, I had to redo the Slack lesson as my AMI did not have all the correct files. I saved another image after all of this and will try to complete the lab on another day.

### jira_runbook.md

Checklist
- [x] Plain (unscoped) API token created, stored privately, expiry date noted.
- [x] Jira variables merged into the existing .env; Slack variables still present; chmod 600 .env.
- [x] python3 jira.py --verify reports the correct project key and name.
- [x] python3 jira.py --test printed a ticket URL; the ticket opens in the browser.
- [x] The same ticket is visible on your board (or you found it in the Backlog and know why).
- [x] python3 incident.py --test shows jira_created: true and slack_status: sent.
- [x] The Slack alert's Jira link opens the ticket created by that same test.
- [x] No token, webhook, or .env contents in screenshots, Git, or chat.

## Homework

- Create your space: SEIR-Saga_Corey, key = SSC
- Turn on Story points
- Build your day: 
> 1 Epic
> at least 5 Stories
> at least 20 Tasks
> every story and task gets a Story point estimate
> every story and task gets a descriptions of at least two sentences

The screenshots folder has the screenshots asked for this homework assignment.

### Evidence Table
| Title | Key | Type | Summary | Story Points |
| --- | --- | --- | --- |
| Morning | SSC-2 | Story | Morning is a time to get up and prepare to face the day. The first part is spent trying to get my mind right and then focus on the body next. | 3 |
| [Morning] Bathroom | SSC-7 | Subtask | Spend a few minutes saying my thanks for being alive. Check myself out in the mirror, prepare for all to see my inner and outer beauty. | 1 |
| [Morning] Meditate | SSC-8 | Subtask | I will spend 10 or so minutes in quiet meditation. This helps me focus on the tasks for the day ahead and get me in the right mood. | 1 |
| [Morning] Reading | SSC-9 | Subtask | This is a time to reflect on some passages for reading, understanding, reflection, affirmations, keep me in the right frame of mind. | 1 |
| Workout | SSC-3 | Story | I begin the day getting my mind right. Now, I focus on getting the body right. This is its own form of meditation. Don’t feel right if I don’t get this in. | 10 |
| [Workout] Warmup | SSC-10 | Subtask | I’ve warmed up my mind at this point, now I have to prepare my body for battle. Perform some breathing exercises, stretching/mobility. Prepare to go outdoors. | 1 |
| [Workout] Cardio | SSC-11 | Subtask | For cardio I go back and forth between cycling and walking. Get the blood pumping, makes me feel most alive. | 2 |
| [Workout] Pushups | SSC-12 | Subtask | I still do this from back in my Army days. It keeps me strong and allows for variety in methods. | 2 |
| [Workout] Pull ups | SSC-13 | Subtask | I didn’t used to do this much, but now that I climb I do it more. Still contributes to multiple body parts. | 1 |
| [Workout] Box jumps | SSC-14 | Subtask | This gets my legs a little more dynamic, focusing on strength. The box isn’t too high now as my vertical isn’t what it used to be. | 1 |
| [Workout] Hangboard abs | SSC-15 | Subtask | Like I said, I’m a climber so I appreciate that little time I get on the wall with others. And this helps round out my workout. | 1 |
| [Workout] Shower | SSC-16 | Subtask | I enjoy this time after a good long workout. This also helps me calm back down to do regular tasks. | 2 |
| Lunch | SSC-4 | Story | Since this is the main meal, I have to get this right. It is composed of homemade dishes from around the world. I used to have a personal chef, but dismissed them after I gained a little freedom and knowledge in the kitchen. | 10 |
| [Lunch] Prepare meat | SSC-17 | Subtask | I eat only once a day, so lunch is critical. Focusing on meat as a main ingredient, but it always needs to be present. | 3 |
| [Lunch] Prepare salad | SSC-18 | Subtask | The other component in my meal is loosely referred to as salad, but it does not have to be a traditional salad, but some form of mixed vegetables. | 3 |
| [Lunch] Prepare smoothie | SSC-19 | Subtask | I know I said I have only one meal, but I do also prepare one snack - usually in smoothie format. Nothing extravagant, just a way to satisfy my sweet tooth and getting in some extra calories if needed. | 1 |
| [Lunch] Eat | SSC-20 | Subtask | Yeah, I get to eat. Can also spend a little time reading the newspaper, browsing the internet, spend a little down time. | 2 |
| [Lunch] Cleanup | SSC-21 | Subtask | Boring, but productive. Just do it. | 1 |
| Volunteer | SSC-5 | Story | It makes my heart feel good to volunteer my time helping others. You gotta give back! | 6 |
| [Volunteer] Help Neighbor | SSC-22 | Subtask | Sure it’s biblical, but it helps not only you by being the helpful person you are to others and they in turn extend the same courtesy to you. | 3 |
| [Volunteer] Feed the needy | SSC-23 | Subtask | No one deserves to go hungry. I have time, slash other things I can give to others, just do it. | 2 |
| [Volunteer] Boys & Girls Club | SSC-24 | Subtask | Again, it’s about treating your neighbor right and if you treat the young right, they’ll grow up to be productive and treat you right. | 1 |
| Evening | SSC-6 | Story | I love the mornings, but this is still a significant part of my day. I’m putting in the work for a better tomorrow, while also memorializing in concurrently. | 7 |
| [Evening] SEIR Homework | SSC-25 | Subtask | The most important part of my day. I got to put in the work to reap the benefits later. Go brothers! | 5 |
| [Evening] Autobiography | SSC-26 | Subtask | I didn’t think I used to have that much to talk about, but when I sat down to think about it, I wanted to share it with others. | 1 |
| [Evening] Prepare for bed | SSC-27| Subtask | Got to get to bed sometime in the evening. Working on the autobiography isn’t too taxing so not hard to wind down. Sweet dreams. | 1 |
| --- | --- | --- | --- | 36 Story total |

The biggest task is doing SEIR homework. It tends to take a lot of time, and there's always more than I can finish.