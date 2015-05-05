# udacity-tournament-results

An exercise in Python and PostgreSQL.

Coordinate and track results for Swiss-style game tournaments using Python 2 and a PostgreSQL database.

## Initialization
Log into your web server via SSH and be sure to have **Python 2** and **PostgreSQL** installed.

To initialize the required tables, run:

```
$ psql
```
```
$ \i tournament.sql
```

## Tables available

**PLAYERS**
Includes the player's name and ID number.

**MATCHES**
ALL match results are recorded here with a match ID numer and the resulting winner or loser.

**VIEW_WINS** _view_
Keeps track of the number of wins for each player.

**VIEW_LOSSES** _view_
Keeps track of the number of losses for each player.

**VIEW_MATCHES** _view_
Keeps track of the count of matches each player has played.

## Running a game

To begin setting up a game:

method | accepts | purpose
registerPlayer(name) | _name as string_ | Adds a player to the database to be calculated in pairings and standings.
countPlayers() | (no input) | Counts all registered players.
