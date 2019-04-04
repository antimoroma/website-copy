### Reasonable Solutions
```kotlin
fun twofer(who: String = "you") = "One for $who, one for me."
```

Another solution could be
```kotlin
fun twofer(who String?) "One for ${name ?: "you"}, one for me."
```
This solution accept a null value for who , and using the "Elvis" operator resolve the interpolation.
Our requisit is "However, if the name is missing, return the string:" and missing coul be non only an empty string , but either a null value. In this case another test need to be created to test the null case

### Common suggestions
* Use default argument values to avoid having to check for null value.
* Curley brackets are not required when embedding variables using string interpolation. Use them only when embedding an expression.
