# Storage
The storage class is used to store data from the game permanently, data that can be accessed again when the game is booted a next time. Keep in mind that this data is stored between sessions of the game in the same machine, but it will not store data across multiple clients, so it is not suited for online games.

## Saving data
In the storage, data is stored as key-value pairs, much like in a Hash Map.
To update data already in the storage, you can also use the _put_ method.
```java
// This will create a storage space that stores the value inside the points value
Storage.put("score", points);
```

If space is a concern, to erase data from the storage the _flush_ method can be used, it will erase a specific pair from the storage.
```java
Storage.flush("score");
```

To erase all the data stored, the _clear_ method may be used.

## Getting data
To retrieve the data stored, the get method can be used, it returns a *Pair<>* value, with the key being the status and the value being the value.
There are five different status:
* VALUE
* EMPTY
* UNIDENTIFIABLE
* SUCCESS
* ERROR

```java
if(Storage.get("score").getValue() < score){
	Storage.put("score", score);
}
```

## Clusters
There may be situations where a key-value pair is not enough to store all the information conveniently, like when we need to store a 4 value RGBA colour, or an X Y position, to create those data structures you may use clusters.

They can be created with a name and a capacity.

```java
Storage.CreateCluster("name", 4);
```

last edited: **10/01/2023**