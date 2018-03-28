# Make or Break - A.I. Competition

The A.I. competition will have 2 main phases:
* Training phase
* Competing phase


## Training phase

The training phase is the initial phase where participants will start
developing their agents before the real competition begins.

In this phase, players are not ranked, and will only get a performance report
of their latest competing bot. This performance report will include the
performance of every match against all other participants’ bots.

This phase will run until April 10th, at 2am.


## Competing phase

The competing phase is where the real competition begins.

Starting April 10th, sets of ranked matches will be played every day, until April 15th:

* April 10th at 2am (Tuesday)
* April 11th at 2am (Wednesday)
* April 12th at 2am (Thursday)
* April 13th at 2am (Friday)
* April 14th at 2am (Saturday)
* April 15th at 2am (Sunday)

After each set of ranked matches, bots will be ranked by their matches’
performance average (day performance).

After the latest set of matches, on April 15th at 2am, we will determine the
winner based on their performance. However, the last day’s performance will
only be revealed in the event’s ending session.

Participants can (and should) keep improving their bots, by submitting new
versions from day to day.

**The latest competing bot submitted by the time the ranked matches begin will
be used in that day’s ranked matches.**


## Performance

Performance is the indicator used to rank bots. There are 3 different types of performance:

* Match performance
* Day performance
* Competition performance


### Match performance

A match is game between two bots from different participants. To calculate the
match performance between Bot A and Bot B:

* Execute a game between Bot A and Bot B
* By the end of the game, count the percentage of squares painted by Bot A and
  the percentage of squares painted by Bot B, in relation to the size of the
  board.
* Add 10% to the bot with the greatest percentage of painted squares, or 5% to
  each bot in the case of a draw (this may go over 100%, and that is fine)
* The higher the percentage, the better the performance


### Day performance

The day performance is the average performance for every ranked match played by
a bot on a given day.

From April 10th to 13th, bots will have to play the same two boards per day.
That means each participant will 2 ranked matches (one on each board) against
every other participant.

On April 14th and April 15th participants will only play a single board, a new
and different one on each day.


### Competition performance

Competition performance will determine the eventual winner of the competition.

Competition performance is calculated by adding:

* The day performance of the last competing day (April 15th)
* The bonus performance gained on early days, according to the following table:

|            | April 10 | April 11 | April 12 | April 13 | April 14 |
|  --------- | -------- | -------- | -------- | -------- | -------- |
|  1st place |     0.5% |     0.8% |     1.1% |     1.4% |     1.7% |
|  2nd place |     0.4% |     0.6% |     0.9% |     1.2% |     1.4% |
|  3rd place |     0.3% |     0.4% |     0.7% |     0.9% |     1.1% |
|  4th place |     0.2% |     0.3% |     0.5% |     0.6% |     0.8% |
|  5th place |     0.1% |     0.2% |     0.3% |     0.4% |     0.5% |
| +6th place |     0.0% |     0.0% |     0.0% |     0.0% |     0.0% |

Example: Kate had the following performance throughout the competing phase:

* April 10 — didn't enter the competition: 0.0%
* April 11 — day performance 30%, 6th place: 0.0%
* April 12 — day performance 34%, 5th place: 0.2%
* April 13 — day performance 50%, 3rd place: 0.9%
* April 14 — day performance 54%, 2nd place: 1.4%
* April 15 — day performance 40%

The competition performance of Kate will be calculated as follows:

```
 0.0% (N/A, April 10) +
 0.0% (6th, April 11) +
 0.2% (5th, April 12) +
 0.9% (3rd, April 13) +
 1.4% (2nd, April 14) +
40.0% (day performance, April 15) = 42.5% competition performance
```

## Submission

To participate in the Make or Break competition, a participant must submit a
bot indicating it is entering the competition.

All submitted code must be authored by the participant and it is considered to
be open-source and under the [MIT License](https://opensource.org/licenses/MIT).

After the competition ends, the organizers will create a repository with all
created bots and their authors, as a record of the competition for the future.

After submitting their bot, participants will get a performance report of their
bot.

## Submission and performance in the training phase

In the training phase, after submitting a bot, the participant will get their
bot’s match performance against all latest created competing bots.


## Submission and performance in the competing phase

In the competing phase, after submitting a bot, the participant will get their
bot's match performance against all other bots submitted to the previous set of
ranked matches, or the latest competing bot, if the other participant still
didn't participate in any ranked matches.
