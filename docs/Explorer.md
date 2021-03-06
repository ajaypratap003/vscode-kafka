# Explorer

The Kafka explorer shows configured clusters with their topics, brokers, consumers and configurations.

![Screenshot-1](assets/screen-1.png)

![Screenshot-2](assets/screen-2.png)

![Screenshot-3](assets/screen-3.png)

## Cluster Item

In the Kafka explorer, right-click on a cluster to access several options.

### Select Cluster

Before using a [.kafka file](KafkaFile.md#kafkafile), a cluster must be selected, you can use the `Select cluster` menu item:

![Select cluster](assets/kafka-explorer-select-cluster.png)

## Actions

### Copy Label

You can copy the label of any tree node in the clipboard with `Ctrl+C` (`Cmd+C` on Mac) or  via the `Copy Label` contextual menu:

![Copy Label](assets/kafka-explorer-copylabel.png)

### Delete

You can delete clusters, topics and consumer groups with the `Delete` (`Cmd+Delete` on Mac) key, the `Trashcan` icon or `Delete` contextual menu:

![Delete Consumer Group](assets/kafka-explorer-delete-consumergroup.png)

Multiple delete is not supported for the moment. See [issue 107](https://github.com/jlandersen/vscode-kafka/issues/107).

To delete a consumer group, it first must be stopped, else the `Delete` action will report an error.

## Preferences

### `kafka.explorer.topics.sort`

Choose sorting for topics in explorer.

### `kafka.explorer.topics.filter`

Glob patterns filtering topics out of the Kafka explorer. `*` matches any string, `?` matches a single character.

### `kafka.explorer.consumers.filter`

Glob patterns filtering consumer groups out of the Kafka explorer. `*` matches any string, `?` matches a single character.