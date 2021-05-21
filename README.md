# Wikipedia-languages-wikibreaks-user-warnings-analysis

Some statistics about languages, wikibreaks and user warnings

## Data format

The data used to generate the charts notebooks are obtained from the [`Wikidump`](https://github.com/samuelebortolotti/wikidump) scripts.

The data structure is fully documented in the `docs` folder of the repository.

## Notebooks

Brief description of the notebooks content

### The `languages` folder

#### About languages

A user on Wikipedia can specify the language he or she knows with a confidence number associated to it by using the [`Babel`](https://en.wikipedia.org/wiki/Template:Babel) template (or similar ones).

The confidence level associated to a language uderstood by a wikipedian are the following ones: `[0, 1, 2, 3, 4, 5, N]`

The knowledge level goes from 0, which is the minimum level, up to N, which is the native speaker level.

For the sake of semplicity, in the data retrieved from the `Wikidump` scripts, the native speaker level `N` has been replaced with the number `6`. 

#### Notebooks content

The notebooks (one for each language) contain the following charts:

* A line chart which represents the fifty languages with the highest number of occurrences.
* A pie chart which represents the percentage of the languages with the highest number of occurrences.
* A line chart which represents the pairs, language - level of knowledge, with the highest number of occurrences

For each knowledge level: 0, 1, 2, 3, 4, 5 and 6:

-   A bar chart which represent the language with the highest number of occurrences.
-   A pie chart which represents the percentage of the languages with the highest number of occurrences.

### The `wikibreak` folder

#### About wikibreaks

A user on Wikipedia can specify a temporary or a permanent break from the platform.

There are several templates for declaring a pause. 
To specify the reasons of a pause, if not implied by the template, it is possible to set different parameters.

Unfortunately the templates and their documentation change from language to language.

#### Notebooks content

The notebooks (one for each language) contain the following charts:

* A pie chart which represents the percentage of the users who currently are in wikibreak.
* A pie chart which represents the percentage of the users who went in wikibreak, compared to the ones who have been active during their wikilife (at least 5 edits in a month)
* A pie chart which represents the most used wikibreaks templates.
* A line chart which shows the amount of users who went in break normalized by the number of active users in those months
* A bar chart which shows the number of times a wikibreak was mentioned
* A pie chart which shows the number of users who went multiple times in wikibreak
* A pie chart which shows the number of users who went multiple times in wikibreak using the same template
* A pie chart which shows the number of users who went multiple times in wikibreak using the same template
* A bar chart for each template which shows the most used parameters
* Some wikibreaks parameters in textual form

### The `user_warnings` folder

#### About user warnings

In Wikipedia user warning template can be used to report malicious actions or to write a customized message on a user's talk page.

There are several user warnings and each of them describe different scenario.

#### Notebooks content

The notebooks (one for each language) contain the following charts:

* A bar chart which shows the number of warnings registered, divided by category
* A line chart which shows the user warnings received over the months
* A bar chart which shows the most used user warnings templates
* A line chart which shows the transcluded user warnings templates over the months
* A line chart which the transcluded user warnings templates over the months
