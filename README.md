# Rate Limiter Middleware

> Token bucket rate limiter for HTTP services — portable Go module.

## Features
- Token bucket algorithm (allows bursting)
- Per-IP rate limiting with configurable capacity/rate
- Lightweight, zero external dependencies

## Usage

```go
import limiter "github.com/farazeool/rate-limiter-middleware"

l := limiter.NewLimiter()
handler := l.Middleware(100, 10)(myHandler)
```

## Why I built this

A simple, correct rate limiter using the token bucket algorithm.

— Faraz

## License
MIT — © 2026 Faraz Mustafa Seyed