```go
func increment() {
	mu.Lock()
	defer mu.Unlock()

	counter++
}
```

100 горутин запустились
горутина #12 первая вызвала Lock
остальные горутины будут дожидаться Unlock
горутина #56 вызовет Lock
...

способ избежать data race

[[RWMutex]]