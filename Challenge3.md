# Challenge 3

## Situation
>At ACME our users are able to search over millions of products. They do thousands of queries per second, and they want the results fast.
>
>Our catalog is very dynamic and new products are being added continuously.

## Task
				
>*  Which search engine would you use and why?
>*  How would you deploy it?
> *	How would you index them?

## Proposed Solution

Having decided that the **SINGLE SOURCE OF TRUTH* is the Stream Store,
as soon we get updates (which are all new events) we can have *Kafka Connect* with a sink into ElasticSearch using its full-text indexing capabilities.

For deployment of see Architecture Diagram below

![](search.png)



