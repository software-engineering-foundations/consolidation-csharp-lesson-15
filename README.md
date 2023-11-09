# Lesson 15 Independent Challenges

For each of the challenges below, exercise these 4 steps.

1. Synchronous method implementation*
2. Asynchronous method implementation (with Async postfix in name)
3. Simple unit test to verify its working
4. Benchmark test; comparing the performance of Parallel.For class utilizing the asynchronous method vs for loops of the synchronous method.
    * Feel free to use any library or tool suite for this, but comparing & printing execution times as part of NUnit tests would be sufficient.
    * Be nice: mock the [`HttpMessageHandler`](https://stackoverflow.com/questions/36425008/mocking-httpclient-in-unit-tests) to avoid congested traffic to real servers
    * Should you use a `Task.WhenAll` or `Task.WaitAll`, why?
    * Should you use a `Timer` or a `Stopwatch`, why?

## Challenge 1: `Wait`

A method that suspends the current thread for a specified amount of time in milliseconds.

## Challenge 2: `ReadTextFile`

A method that reads contents of a text file as an array of strings, separated by new lines.

## Challenge 3: `GetPokemonData`

A method that fetches a Pokemon's data from [Poke API](https://pokeapi.co/).

Use built-in `HttpClient` for this, task and you may need to do some reading to figure how to do it synchronously.

*calling async methods inside the method is acceptable but no `async` / `Task` for the method signature allowed. This is relevant for Challenge 3.

## Challenge 4: `GetWikipediaEntry`

A method that fetches the first paragraph of the Wikipedia page of given subject. 

Use [HtmlAgilityPack](https://html-agility-pack.net/) for this task.