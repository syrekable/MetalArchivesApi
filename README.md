# Metal Archives API

## About

As there is currently no public [metal archives](https://www.metal-archives.com/) API, the alternative solution must be proposed. Let's scrape the site and make the data free and accessible for the glory of the beast, shall we?

## Schemes - diagram

![Database scheme diagram](/DbScheme.png?raw=true "Database scheme diagram")

## Schemes - description

### Metal Band Scheme

| Column            | Not null |
|-------------------|----------|
| ID                |  ✔       |
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
| ID              | ✔        |
| Name            | ✔        |
| Real/full name  |          |
| Place of origin |          |
| Gender          |          |

### Release Scheme

| Column         | Not null |
|----------------|----------|
| ID             |          |
| Band           |          |
| Title          | ✔        |
| Type           | ✔        |
| Release date   | ✔        |
| Catalog ID     |          |
| Songs          | ✔        |
| Lineup*        | ✔        |
| Format         | ✔        |
| Average rating |          |

\**I'm not sure how to represent a lineup, I'd use some guidance*

### Label scheme

| column           | not null |
|-----------------|-------|
| ID              |       |
| name            |   ✔   |
| status          |   ✔   |
| country         |   ✔   |
| address         |       |
| website         |       |
| specialities    |       |
| founding date   |       |
| online shopping |       |
