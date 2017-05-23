# kafka_tools


## kafka_purge_queue

This tool can be used to purge some kafka topic.

#### Prerequisite:

    brew install kafka

#### Usage:

    ./kafka_purge_queue <topic_name>

#### Example:
```bash
$ ./kafka_purge_queue topic-to-delete
Going to purge kafka topic 'topic-to-delete'...
>>> If you ran this by mistake, press 'Ctrl + C' NOW! <<<
Purging kafka topic topic-to-delete...
Completed Updating config for entity: topic 'topic-to-delete'.
Waiting for message queue to clear...
Setting retention back to default...
Completed Updating config for entity: topic 'topic-to-delete'.
```

#### Parameters
Wait time for cluster to converge:

    WAIT=300 # 5 min

Generally a few minutes are good enough, but for large topic or some network issues, you may want to put a larger wait time.
