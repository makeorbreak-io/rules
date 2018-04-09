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

This phase will run until April 10th, at 02:00.


## Competing phase

The competing phase is where the real competition begins.

Starting April 10th, sets of ranked matches will be played every day, until April 15th:

* April 10th at 02:00 (Tuesday)
* April 11th at 02:00 (Wednesday)
* April 12th at 02:00 (Thursday)
* April 13th at 02:00 (Friday)
* April 14th at 02:00 (Saturday)
* April 15th at 02:00 (Sunday)

Please keep in mind that those times are 2 hours after the day has started.
That means that the first set of ranked matches is played 2 hours after April
9th has ended. Be sure to submit your bot in time.

After each set of ranked matches, bots will be ranked by their matches’
performance average (day performance).

After the latest set of matches, on April 15th at 02:00, we will determine the
winner based on their performance. The last day’s performance will only be
revealed in the event’s ending session.

Participants can (and should) keep improving their bots, by submitting new
versions from day to day.

**The latest competing bot submitted by the time the ranked matches begin will
be used in that day’s ranked matches.**


## Performance

Performance is the indicator used to rank bots. There are 4 different types of
performance (higher is better):

* Game performance
* Match performance
* Day performance
* Competition performance


### Game performance

Game performance is a bot's individual performance in a game in which it took part.
The game may be played by N bots from different participants. Game performance is calculated
at the end of the game, as follows:

1. Calculate the percentage of squares painted by the bot in relation to the size of the board. The resulting value is the number of base points of a bot. If the value is a float, it is truncated (e.g. 70.1 and 70.9 both become 70);
1. Calculate the number of base points for each of the N bots that played the game;
1. If there is a single bot with the highest number of base points, award it 10 extra points;
1. If there are multiple bots with the highest number of base p oints, award each bot 5 extra points;
1. The game performance is the number of base of points plus the number of extra points.

### Match performance

A match is a set of M games. The match performance of a bot is the average game
performance for the M games played. To reduce match performance variance, M
should be greater than 1. Howeever, to simplify things, in this year's
competition, M equals 1, making match performance equal to game performance.


### Day performance

The day performance is the average performance for every ranked match played by
a bot on a given day (sum of all the matches performance over the number of
matches). From April 10th to 13th, bots will have to play two different boards
per day (board sizes will differ, as well as the number of turns and starting
positions; the initial board may also have prepainted squares). That means each
participant will have 2 ranked matches (one on each board) against every other
participant.

On April 14th and April 15th participants will only play a single board, a new
one on each day.


### Competition performance

Competition performance will determine the winner of the competition.

Competition performance is calculated by adding:

* The day performance of the last competing day (April 15th)
* The bonus performance gained on early days, according to the following table:

|            | April 10 | April 11 | April 12 | April 13 | April 14 |
|  --------- | -------- | -------- | -------- | -------- | -------- |
|  1st place |     0.5  |     0.8  |     1.1  |     1.4  |     1.7  |
|  2nd place |     0.4  |     0.6  |     0.9  |     1.2  |     1.4  |
|  3rd place |     0.3  |     0.4  |     0.7  |     0.9  |     1.1  |
|  4th place |     0.2  |     0.3  |     0.5  |     0.6  |     0.8  |
|  5th place |     0.1  |     0.2  |     0.3  |     0.4  |     0.5  |
| +6th place |     0.0  |     0.0  |     0.0  |     0.0  |     0.0  |

Example: Kate had the following performance throughout the competing phase:

* April 10 — didn't enter the competition: 0.0 bonus points
* April 11 — day performance 30 points, 6th place: 0.0 bonus points
* April 12 — day performance 34 points, 5th place: 0.2 bonus points
* April 13 — day performance 50 points, 3rd place: 0.9 bonus points
* April 14 — day performance 54 points, 2nd place: 1.4 bonus points
* April 15 — day performance 40 points

The competition performance of Kate will be calculated as follows:

```
 0.0 (N/A, April 10) +
 0.0 (6th, April 11) +
 0.2 (5th, April 12) +
 0.9 (3rd, April 13) +
 1.4 (2nd, April 14) +
40.0 (day performance, April 15) = 42.5 competition performance
```

## Winners

The three winners of the competition will be the participants with the highest
**competition performance**. We will use the sum of the players’ sixth **day
performances** to break any ties.

In Kate’s example, the tie breaking value would be 0 + 30 + 34 + 50 + 54 + 40 =
**208 points**. If this is not sufficient to resolve ties, the organizing team
reserves the right to arbitrate new tie breaking mechanisms during the final
competition day.

## Submission

To participate in the Make or Break competition, a participant must submit a
bot indicating it is entering the competition.

All submitted code must be authored by the participant and it is considered to
be open-source and under the [MIT License](https://opensource.org/licenses/MIT).

After the competition ends, the organizers will create a repository with all
created bots and their authors, for archival purposes.

After submitting their bot, participants will get a performance report of their
bot.


## Submission and performance in the training phase

In the training phase, after submitting a bot, the participant will get their
bot’s match performance against the latest versions of all other competing
bots.


## Submission and performance in the competing phase

In the competing phase, after submitting a bot, the participant will get their
bot’s match performance against the latest versions of all other competing
bots.

**This is not the performance that will be used to calculate the ranked day
performance. The organizing team will release the official daily leaderboards.**
