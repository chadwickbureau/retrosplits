# retrosplits

This dataset contains historical playing data from Major League Baseball (tm),
disaggregated at various levels.  These are based on the files
produced by Retrosheet. 

There are two main groupings of files:
* daybyday: Game-by-game records for players and teams, for all seasons
  available from Retrosheet.
* splits: Various batting and pitching splits generated from event-level
  data, that is, which cannot be computed from the game-by-game records.
  This covers 1974 through present, for which Retrosheet has full
  play-by-play coverage.

The daybyday files include records from Retrosheet event files,
deduced event files, and boxscore files.  If Retrosheet offers a game
in more than one of these types of file, then there will be multiple
records for the players and teams in that game.  There is a column
'game.source' which indicates the source of the record:
* evt: event file
* ded: deduced event file
* box: boxscore file

Retrosheet proofs games closely for offensive and pitching statistics.
Defensive statistics, specifically putouts and assists, are less
closely proofed, as these are known to be much less reliably kept, and
because scorecards often have missing or inaccurate data for these.
Generally boxscore files reflect official totals, while event files
will reflect the limitations of the known sources of play-by-play for
the game in question.

Deduced event files are play-by-play files which are reconstructed
from partial information and context, rather than complete or almost
complete game accounts.  Some statistical categories may therefore be
unreliable in these accounts.

We include the statistical totals derived from each of these sources
because they have relative strengths; for example, plate appearances
are not included in boxscore files, but in most cases can be computed
accurately from event files.  Users will need to choose which
source(s) to use for their own work.

The underlying data is obtained free of charge from and is copyrighted
by Retrosheet.  Interested parties may contact Retrosheet at
www.retrosheet.org.

This dataset is made available under the Open Database License:
http://opendatacommons.org/licenses/odbl/1.0/. Any rights in
individual contents of the database are licensed under the Database
Contents License: http://opendatacommons.org/licenses/dbcl/1.0/.

The maintainer of this dataset is Dr Theodore Turocy, Chadwick
Baseball Bureau; ted.turocy@gmail.com / http://www.chadwick-bureau.com.
