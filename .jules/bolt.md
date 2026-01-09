## 2024-03-27 - [JSON Parsing Performance]
**Learning:** `json.loads` on incomplete data inside a socket loop causes quadratic complexity (O(N^2)) when buffering large payloads, because the entire buffer is decoded on every chunk.
**Action:** Always check `buffer.strip().endswith(b'}')` before attempting to parse JSON from a socket buffer. This simple O(N) check prevents the expensive decode/parse operation until the data is likely complete.
