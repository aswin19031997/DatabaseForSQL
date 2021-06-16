# Database For Chess Organization
#Business Rules: (Relationship, Attribute, Constraints, Entity) 

Each player can only have membership of one chess club, but every chess club can have multiple players. 

Every player of the club has a unique player id, and every club has a unique club id.  

Players participating in the tournament may or may not have a fide rating. 

Players banned can’t attend this tournament. 

Every chess club should have at least one player  

During tournament chess clubs accept donations from their sponsors. 

There can be many sponsors for the tournament chess club.  

Each sponsor can donate to only one chess club.  

A tournament can have multiple categories, but each category will have its own tournament. 

Each player can participate only in one category.  

Each game has to be monitored by the referee and referee may monitor many games during the tournament.  

Each referee should have a rating above fide rating 1500. 

For each matchup, the player winning the game will get one point, player who loses gets zero point, and If it’s a draw, players get half point each. 

Rank of player in each tournament is important and each player have their own ranking level.   

Players are ranked based on the points they secure in the tournament.  

Each tournament can have many matchup but match up can be a part of only one tournament  

 

#Entity: 
Player, Club, Category, Sponsor, Sponsorship, Game, Tournament, Ranking, Matchup, Referee. 

#Attributes : 

Player: player_id, rank_level, player_name, fide_ranking, banned   

Club: club_id, club_name, club_owner, club_location 

Category: category_id, category_name 

Game: game_id 

Sponsor: sponsor_id, sponsor_name 

Sponsorship: Amount,sponsorship_id  

Tournaments: tour_id, date, venue, location, tour_name 

Referee: referee_id, ref_name, fide_rating 

Match-up: points 

Ranking: rank_id,  total_points. 

 

#Relationships: 

Players are part of a club 

Sponsors provide sponsorship to club and  to a tournament  

Refree monitors the games 

Player has ranking  

Player is a part of a category  

Player has match-up 

Category is a part of the tournament  

Tournament has  match up  

 
