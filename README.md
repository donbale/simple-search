A simple search engine that runs on Node.JS, Express and MongoDB. It support basic document indexing and querying.

## Installation
```npm install simple-search```

## Usage

You can use the search engine either via a REST API using HTTP requests.

###RESTful API

** Indexing **
/index

** Searching **
/search

###Command line

** Crawling **

You can start the crawler using ```simple-crawl -s <the_start_url>```

```
$ simple-crawl --help

  Usage: simple-crawl [options]

  Options:

    -h, --help                 output usage information
    -V, --version              output the version number
    -s, --starturl <starturl>  The initial url
```

## Design Choices

**Promises**
Promises are used for readability and proper error handling.

**MongoDB**
MongoDB is used in the current version but you can use any other database you wish. You can create an index with another database and pass it to the indexer during construction, as long as you comply with the following API (todo show API here).  