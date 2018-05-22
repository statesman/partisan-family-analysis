# Partisan family analysis

This repo contains analysis supporting the Austin American-Statesman article "[A house divided: Central Texas families who cast opposite votes](https://www.mystatesman.com/news/state--regional-govt--politics/house-divided-central-texas-families-who-cast-opposite-votes/tZ4o7Q03x9wQtpjjzcQN9J/)."

### Data

Analysis involved lists of registered voters in Travis, Williamson and Hays counties. The `Registered Voters List Compressed` csv file was downloaded from the [Travis County Tax Office](https://tax-office.traviscountytx.gov/voter-data) site with a last modified date of April 30, 2018. Data from [Williamson](http://www.wilco.org/Departments/Elections/Staff) and [Hays](http://www.co.hays.tx.us/elections.aspx) counties were provided on May 7 in response to requests to the county elections departments.

### Analysis

`analysis.ipynb` calculates "split-voting" or "partisan" families with the following metrics:

Term | Definition
|-----|-----|
`Family` | A combination of an address and a last name where multiple voters with the same last name registered at the same address voted in a March 2018 primary
`Split-voting family` | `Family` where at least one member voted in the March |2018 Republican primary and at least one member voted in the Democratic primary
`Split voting families percentage` | Number of `Split-voting families` divided by the number of `Families`

### Reproducibility

- Ensure that you have installed [Jupyter](http://jupyter.org/), [Python](https://www.python.org/), and the [pandas data-analysis library](https://pandas.pydata.org/).
- Download registered voters from [Travis County](https://tax-office.traviscountytx.gov/voter-data) and request from [Williamson](http://www.wilco.org/Departments/Elections/Staff) and [Hays](http://www.co.hays.tx.us/elections.aspx) counties. Note: results may differ from this repo if lists of registered voters have changed.

### Feedback? Questions?

Contact Dan Keemahill at [dkeemahill@statesman.com](dkeemahill@statesman.com).
