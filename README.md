# Spark-Streaming

# Spark application that consumes events generated by a Python producer in Kafka.

#The Kafka cluster.
• Set the KAFKA_ADVERTISED_HOST_NAME with your docker host IP
• The KAFKA_CREATE_TOPICS configuration creates a topic called wiki-changes with 1 partition
  and 1 replica just for test purposes and you can change it if you want to test with more partitions
   or replicas.

#Spark 
To execute the Spark application interactively, use the Jupyter service with Spark embedded.

To begin producing events from changes in Wikipedia pages to a Kafka topic, run the event-producer.ipynb notebook.
Run the event-consumer-spark.ipynb notebook to begin consuming events from the Kafka topic and writing them to files.
Run the data-visualization.ipynb notebook to read the parquet files in streaming mode and visualise the top ten users with the most edits.
