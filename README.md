### Movie ratings DATA simple preprocessing & Analysis
## File : ratings.dat ,users.dat , movies.dat (in ml-1m directory)

## integrated File :integrated.csv (over 100mb)
## integrated Pandas DataFrame Pickle file : integrated.pkl

### Data Structure
"ratings.dat" UserID::MovieID::Rating::Timestamp
"users.dat"   UserID::Gender::Age::Occupation::Zip-code
"movies.dat"  MovieID::Title::Genres

- UserIDs  1 ~ 6040 
- MovieIDs 1 ~ 3952
- Ratings  5-star scale (whole-star ratings only)
- Timestamp is represented in seconds since the epoch as returned by time(2)

- Gender  "M" ,"F" 
- Age 
	*  1:  "Under 18"
	* 18:  "18-24"
	* 25:  "25-34"
	* 35:  "35-44"
	* 45:  "45-49"
	* 50:  "50-55"
	* 56:  "56+"
- Occupation 
	*  0:  "other" or not specified
	*  1:  "academic/educator"
	*  2:  "artist"
	*  3:  "clerical/admin"
	*  4:  "college/grad student"
	*  5:  "customer service"
	*  6:  "doctor/health care"
	*  7:  "executive/managerial"
	*  8:  "farmer"
	*  9:  "homemaker"
	* 10:  "K-12 student"
	* 11:  "lawyer"
	* 12:  "programmer"
	* 13:  "retired"
	* 14:  "sales/marketing"
	* 15:  "scientist"
	* 16:  "self-employed"
	* 17:  "technician/engineer"
	* 18:  "tradesman/craftsman"
	* 19:  "unemployed"
	* 20:  "writer"


- Titles are identical to titles provided by the IMDB (including
year of release)
- Genres are pipe-separated and are selected from the following genres: 18개

	* Action
	* Adventure
	* Animation
	* Children's
	* Comedy

	* Crime
	* Documentary
	* Drama
	* Fantasy
	* Film-Noir

	* Horror
	* Musical
	* Mystery
	* Romance
	* Sci-Fi

	* Thriller
	* War
	* Western
