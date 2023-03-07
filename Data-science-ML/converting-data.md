## Converting Data

There are some techniques to turn data into tags and 1-Hot Encoding (OHE) to facilitates its manipulation.

For example, we can turn Categoric data into Tags, because we can't really pass this kind of data to the model, so we need it to convert this into numerical data:

#### Categoric

| Day 1 | Day 2  | Day 3 | Day 4 | Day 5  |
| ----- | ------ | ----- | ----- | ------ |
| Sunny | Cloudy | Suny  | Rainy | Cloudy |

#### Into tags with numerical data

Sunny = 1
Cloudy = 2
Rainy = 3

| Day 1 | Day 2 | Day 3 | Day 4 | Day 5 |
| ----- | ----- | ----- | ----- | ----- |
| 1     | 2     | 1     | 3     | 2     |

However, there is another approach called _**One-Hot Encoder**_ or _**OHE**_, where the goal is to create a vector to represent a question asked of each dataset:

```
x = [x1 = sunny, x2 = cloudy, x3 = rainy]

so, the vector of day 2 can be represented as:

xDay2 = [1,0,0] (Day 2 was cloudy)
```
