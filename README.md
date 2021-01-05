## Mocking

Mocking is primarily used in unit testing. An object under test may have dependencies on other (complex) objects. To isolate the behavior of the object you want to replace the other objects by mocks that simulate the behavior of the real objects. This is useful if the real objects are impractical to incorporate into the unit test.

In short, mocking is creating objects that simulate the behavior of real objects.

## Hash table
[hash_table](https://techdic.ir/definition/hash-table/)

## Bloom Filter
[bloom_filter](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwixwY_2xtXtAhWB_CoKHSmPBBEQFjABegQIAhAC&url=https%3A%2F%2Fvirgool.io%2F%40hossein52hz%2F%25D9%2585%25D9%2588%25D8%25AC%25D9%2588%25D8%25AF%25DB%258C-%25D8%25B9%25D8%25AC%25DB%258C%25D8%25A8-%25D8%25A8%25D9%2587-%25D9%2586%25D8%25A7%25D9%2585-bloom-filter-%25D8%25AF%25D8%25B1-%25D8%25A8%25D8%25B1%25D9%2586%25D8%25A7%25D9%2585%25D9%2587-%25D9%2586%25D9%2588%25DB%258C%25D8%25B3%25DB%258C-iajb0fn0ata1&usg=AOvVaw0MkjC8a-1xjltLG9bf26pp)

## Concurrency
[golang pool worker](https://www.youtube.com/watch?v=LvgVSSpwND8)


Concurrency is not the same as parallel programming or parallelism because parallelism is about parallel execution and concurrency is a little bit more bacause Concurrency is about designing your program as a collection of independent processes about designing these processes to eventually run in parallel.
Concurrency is good for your code  if:
* group code(and data) by identifying independent tasks
* no race conditions
* no deadlocks
* more workers = faster execution

Concurrency is aboute breaking up  a program into independently executing tasks could potentially run at the same time and still getting the right result at the end so concurrent program can be parallelized.
In golang you can run methods by go like this

```
fun main(){
 c := make(chan sting)
 go count("ship", c)
 
 msg := <- c
 fmt.Pringln(msg)
 
}
func count(thing string, c chan sting){
    for i := 1; i<5 i++ {
      c <- thing
      time.Sleep(time.Millisecond * 500)
    }
}
```
In this code go means goroutine
