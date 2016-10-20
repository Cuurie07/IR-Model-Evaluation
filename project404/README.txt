#The data is the train.json file containing tweets from English,German and Russian with a format as shown below

##Sample tweet format is as follows:
{
"lang": ,
"id": , 
"text_de": ,
"text_en": , 
"text_ru": , 
"created_at": , 
"tweet_urls": [ ], 
"tweet_hashtags": []
}
#########################################

##You are provided with 14 sample queries (queries.txt ) and corresponding manually judged relevance score (qrel.txt) .

###queries.txt, includes 14 sample queries. One query per line. Each line has format query_number query_text

####q rel.txt, i ncludes manually judged relevance score. Format as shown below

query_number 0 document_id relevance


####the config contains the schema.xml and schemaconfig.xml for the optimal configurations for each of the different models in Solr.

###the BM25,LM and VSM folders contain the output for each model. Each .txt file corresponds to one query. The format of each output file is as follows

#########

query­number Q0 tweet_id rank similarity_score model_name

#########


