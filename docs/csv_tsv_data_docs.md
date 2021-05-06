# Languages

Level of linguistic self-assessment of Wikipedia users based on the latest revision of their user page.

## Structure

| id             | timestamp              | name                                 | uid          | language     | level        |
| :------------- | :--------------------: | -----------------------------------: | -----------: | -----------: | -----------: |
|  0             | 2007-04-24T18:14:54Z   | Llull                                | 5668         | catalan      | 6            |
|  1             | 2007-04-24T18:14:54Z   | Llull                                | 5668         | spanish      | 6            |
|  ...           | ...                    | ...                                  | ...          | ...          | ...          |
|  49            | 2015-04-19T02:21:17Z   | Get-back-world-respect~cawiki        | 11157        | german       | 6            |
|  ...           | ...                    | ...                                  | ...          | ...          | ...          |

The `timestamp` field refers to the latest revision of the user page.

The `id` field indicates the identification number of the csv / tsv entry.

# Wikibreaks

Wikibreaks and its category with the related parameters specified by the user on their user page or on the user talk page.

At each line of the csv / tsv file there is the wikibreak template with the history of the specified parameters 

## Structure

| id | talk_page_id | name      | uid    | ambiguous | wikibreak | categories | parameters                                                     | subcategory | to_date                   |  from_date                   |
| :- | :----------: | --------: | -----: | --------: | --------: | ---------: | -------------------------------------------------------------: | ----------: | ------------------------: |  --------------------------: |
|  0 | 43723        | Pepetps   | 43517  | False     | exàmens   | ['break']  | "[{'options': {}, 'timestamp': '2006-05-21 20:44:26+00:00'}]"  | exams       | 2006-07-08 12:07:34+00:00 |  2006-05-21 20:44:26+00:00   |
|  ... | ...          | ...       | ...    | ...       | ...       | ...        | ...                                                            | ...         | ...                       | ...                        |
|  12 |             | Arbocenc  | 13058  | False     | ocupat    | ['mental'] | "[{'options': {}, 'timestamp': '2007-02-12 18:52:02+00:00'}]"  | busy        |                           |  2007-02-12 18:52:02+00:00   |
|  ... | ...          | ...       | ...    | ...       | ...       | ...        | ...                                                            | ...         | ...                       | ...                        |

The `id` field indicates the identification number of the csv / tsv entry.

The `ambiguous` field specifies whether there was a temporal overlap of the same wikibreak template.

The `categories` field is a list of strings, and the parsing must be done once the data has been extracted, the same must be done for the `parameters` field whose structure is specified in the `json_data_docs.md` file.