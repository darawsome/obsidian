---
cssclasses:
  - cards
  - cards-cover
  - cards-2-3
  - table-max
---
```dataview
table without id 
	("![](" + poster + ")") as Poster,
	file.link as Title,
	string(year) as Year, 
	"by " + director as Director,
	"⭐ " + scoreImdb as "⭐ IMDB",
	rating, genre
from #movies 
where poster != null
where contains(status, "to watch")
```
