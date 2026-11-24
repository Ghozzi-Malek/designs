# Web crawler design

## Functional requirements
- a web crawler should be able to access to websites
- a web crawler should be able to save website as html


## scale (before going to non functional requirements)
- 10B web pages 
- 2 MB per page avg  => ask the intreviewer before on the scale of the system before going to non functional requirements
- 5 days to scrape

- unlimited ressources (ask about the ressources because these things can effect the high level desing)

## Non functional requirements
- Politness (a web crawler should respect robots.txt of every website)
- Fault tolerent (we must not lose our progress if something accured)
- scale to 10B page
- efficiently crawl under 5 days


## Core entities

- url meta data
- text extracted

## interface

- urls => input
- text data => output

## Data flow (the steps that the system will apply on the input in order to get that output)


1) get urls ip from dns
2) fetch html
3) extract from html its html
4) save text in database
5) extract urls that are in the current web page
6) Repeat

## High level design

#### first design


