Java Stream API Cheatsheet
Intermediate Operations:
filter(Predicate):

Use Case: Filters elements based on a specified condition.
Example: Filtering a list of integers to get only even numbers.
map(Function):

Use Case: Transforms each element into another object using the provided function.
Example: Converting a list of Strings to their lengths.
flatMap(Function):

Use Case: Similar to map, but when each element is mapped to a Stream, and the results are flattened into a single Stream.
Example: Flattening a list of lists into a single list.
sorted() / sorted(Comparator):

Use Case: Sorts the elements of the stream either in natural order or using a provided comparator.
Example: Sorting a list of strings alphabetically.
distinct():

Use Case: Removes duplicate elements from the stream.
Example: Removing duplicate entries from a list.
limit(long) / skip(long):

Use Case: Limits the number of elements in the stream or skips a specified number of elements.
Example: Retrieving only the first 5 elements from a stream or skipping the first 3 elements.
peek(Consumer):

Use Case: Performs a consumer action for each element of the stream, primarily useful for debugging or logging.
Example: Logging each element of a stream before further processing.
dropWhile(Predicate) / takeWhile(Predicate):

Use Case: Drops or takes elements from the stream while the predicate condition is true.
Example: Dropping elements from the stream until an element greater than 10 is encountered.
concat(Stream):

Use Case: Concatenates two streams into a single stream.
Example: Concatenating two lists into a single stream.
Terminal Operations:
forEach(Consumer):

Use Case: Performs a specified action for each element of the stream.
Example: Printing each element of a stream.
collect(Collector):

Use Case: Performs a mutable reduction operation on the elements of the stream, accumulating them into a mutable result container.
Example: Collecting elements of a stream into a List or Map.
reduce(identity, BinaryOperator):

Use Case: Performs a reduction on the elements of the stream using the provided binary operator.
Example: Calculating the sum or maximum of elements in a stream.
min(Comparator) / max(Comparator):

Use Case: Finds the minimum or maximum element in the stream, optionally using a provided comparator.
Example: Finding the smallest or largest element in a stream.
count():

Use Case: Returns the count of elements in the stream.
Example: Counting the number of elements in a stream.
anyMatch(Predicate) / allMatch(Predicate) / noneMatch(Predicate):

Use Case: Checks if any, all, or no elements of the stream match a given predicate.
Example: Checking if any element is greater than 10 or if all elements are positive.
findAny() / findFirst():

Use Case: Finds any or the first element of the stream.
Example: Finding any element greater than 5 or finding the first element of a stream.
toArray() / toArray(IntFunction):

Use Case: Collects the elements of the stream into an array.
Example: Converting a stream of integers into an array.
forEachOrdered(Consumer):

Use Case: Performs an action for each element of the stream, maintaining the order of encounter.
Example: Printing each element of a stream in the order of encounter.