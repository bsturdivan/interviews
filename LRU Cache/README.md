# LRU Cache

**Part 1 — Algorithm**
Implement an LRU cache: `get(key)` and `put(key, value)` both O(1), fixed capacity, evict least-recently-used on overflow. Hash map + doubly-linked list is the expected shape.

**Part 2 — Expand with AI**
Wrap it as a caching layer in front of an async data source: `getOrFetch(key, fetchFn)`. Add TTL expiry, then handle the stampede case (N concurrent calls for a cold key should trigger one fetch, not N). Add stats (`hits`, `misses`, `evictions`). The concurrency dedup is where AI output looks right and isn't — make it prove the single-fetch guarantee with a test.
