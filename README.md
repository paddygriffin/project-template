# Irish Constituencies Neo4j Database
###### **Patrick Griffin**, **G00314635**

## Introduction
This project is a database(Neo4j) collected of *candidates*,*constituencys*,*parties* and their *relationships* in the 2016 election of Ireland. 

## Database
Firstly, I created the 40 constituencies with a brief description of each constituency. Here is an example of how to create one:
```
create (`nCork South-West`:Constituency {name:"Cork South-West", population:82952, seats:3, description:"The county of Cork, except the parts thereof which are comprised in the constituencies of Cork East, Cork North-Central, Cork North-West, and Cork South Central."})
```

**Properties include**
* name
* population
* seats
* description

Next, I created the candidates based on their constituency and entered each of their properties. Here is an example:
```
Create (`nDarragh O'Brien`:Candidates {name:"Darragh O'Brien", party:"Fianna Fail", gender:"Male", constituency:"Dublin Fingal", age:41, elected:"yes"}),
(`nClare Daly`:Candidates {name:"Clare Daly", party:"Independents 4 Change", gender:"Female", constituency:"Dublin Fingal", age:47, elected:"yes"})

```
If a candidate has no information for age as an example I entered **null** as its value. I also show if the candidate was elected or not.
Here are the candidates properties:
* name
* party
* gender
* constituency
* age
* elected

## Queries
Summarise your three queries here.
Then explain them one by one in the following sections.

#### Query one title
This query retreives the Bacon number of an actor...
```cypher
MATCH
	(Bacon)
RETURN
	Bacon;
```

#### Query two title
This query retreives the Bacon number of an actor...
```cypher
MATCH
	(Bacon)
RETURN
	Bacon;
```

#### Query three title
This query retreives the Bacon number of an actor...
```cypher
MATCH
	(Bacon)
RETURN
	Bacon;
```

## References
1. [Neo4J website](http://neo4j.com/), the website of the Neo4j database.
2. https://en.wikipedia.org/wiki/Parliamentary_constituencies_in_the_Republic_of_Ireland
3. http://www.thejournal.ie/election-2016/constituency/26/
