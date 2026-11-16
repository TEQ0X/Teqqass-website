MULTI-WORKER CLONING
- Bulk clone: 20 parallel workers (CLONE_WORKERS)
- Car inject inside one clone: up to 16 parallel saves (CAR_CLONE_WORKERS)
- Shared HTTPS keep-alive pool: 400 connections, sized for the existing parallel-save ceiling to reduce connection setup overhead.
- Bulk limit: user 300 / admin 500
- Progress: "Workers=20 · N/M done"
- Bulk account registration retries up to 5 times; target profile transfer retries up to 3 times.
- Car saves retry transient failures; the garage is read back and missing cars are retried twice before the job reports completion.
- The final job summary distinguishes fully completed clones from accounts needing attention.
