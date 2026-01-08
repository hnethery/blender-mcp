## 2025-05-20 - Poly Haven API Limitation
**Learning:** The Poly Haven API does not support pagination or server-side filtering (limit/count) for the `/assets` endpoint. It returns the entire database of assets (metadata), which forces the client to download a large payload and filter it locally. This is a potential performance bottleneck for asset searching.
**Action:** In future, if asset search becomes too slow, consider caching the asset list locally or using an intermediate proxy service if possible. For now, we filter in Python after downloading.
