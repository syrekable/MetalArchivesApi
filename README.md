# Metal Archives API

## About

As there is currently no public [metal archives](https://www.metal-archives.com/) API, the alternative solution must be proposed. Let's scrape the site and make the data free and accessible for the glory of the beast, shall we?

## Schemes *(4/5 tables ready)*

### Metal Band Scheme

| Column            | Not null |
|-------------------|----------|
| BandID            |          |
| Name              |  ✔       |
| Country of origin |  ✔       |
| Location          |  ✔       |
| Status            |  ✔       |
| Formed in         |          |
| Years active      |          |
| Genre             |  ✔       |  
| Lyrical themes    |          |
| Last label        |  ✔       |

### Artist Scheme

| Column          | Not null |
|-----------------|----------|
| ArtistID        | ✔        |
| Name            | ✔        |
| Real/full name  |          |
| Place of origin |          |
| Gender          |          |

### Release Scheme

| Column         | Not null |
|----------------|----------|
| ReleaseID      |          |
| Band           |          |
| Title          | ✔        |
| Type           | ✔        |
| Release date   | ✔        |
| Catalog ID     |          |
| Songs          | ✔        |
| Lineup         | ✔        |
| Format         | ✔        |
| Average rating |          |

### Label scheme

| column           | not null |
|-----------------|-------|
| LabelID         |       |
| name            |   ✔   |
| status          |   ✔   |
| country         |   ✔   |
| address         |       |
| website         |       |
| specialities    |       |
| founding date   |       |
| online shopping |       |
