mmsProject1Blog
================
Maxwell Marion-Spencer
2022-06-26

## Project 1 Blog Post

For ST 558 Project 1 I created a vignette for
[PokeAPI](https://pokeapi.co/).

In this vignette I created a number of functions that would allow a user
to more easily request data from the API, and to have said data returned
in a usable data frame form. Specifically, I created functions for the
`pokemon`, `habitat`, `color`, `egg-group`, and `berry` endpoints. For
each function it was important to adapt the query to the users’
potential input.

For the `pokemon` and `berry` endpoints, I also included an option to
bring down the entire contents of the endpoint, as this might be useful
for someone doing data analysis.

As far as my own analysis of the data I pulled down - I was particularly
surprised to find that there wasn’t any apparent relationship between
the size of a berry and the growth_time. Other fun findings included
discovering that fighting type pokemon are apparently particularly dense
and ghost pokemon are on average very light, after creating a BMI
statistic and doing quantitative analysis on the mean, median, and
standard deviation of pokemon’s height, weight and BMI.

The most difficult part of the logic and programming was the initial
hurdle of considering how to get the data in and fit into a data frame.
I ended up creating a row of blank values (deleting them afterwards) and
using `rbind()` in order to loop through API queries and append them to
my desired data frame. I’m sure that there was probably a better way but
I was enthused when my solution worked!

Doing a similar project in the future, I would probably just try to
spend less time fretting about how exactly I was going to implement
every last detail and simply jump in and get started. I spent a lot of
time trying to think of everything at once.

To view my project click either link below!

Github Pages Repo: <https://maxwell-marion.github.io/project1-558/>

Regular Github Repo: <https://github.com/maxwell-marion/project1-558>
