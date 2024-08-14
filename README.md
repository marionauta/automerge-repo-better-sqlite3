# automerge-repo-better-sqlite3

An [automerge][automerge] [repo][automerge-repo] storage adapter that uses
[better-sqlite3][better-sqlite3] to store documents.

This project is a fork of [this repo][original].

## Usage

```typescript
import { Repo } from "@automerge/automerge-repo";
import { BetterSqlite3StorageAdapter } from "@marionauta/automerge-repo-better-sqlite3";
import Database from "better-sqlite3";

const db = new Database();
const repo = new Repo({
  storage: new BetterSqlite3StorageAdapter(db),
  // ...
});
```

[automerge]: https://automerge.org
[automerge-repo]: https://github.com/automerge/automerge-repo
[better-sqlite3]: https://github.com/WiseLibs/better-sqlite3
[original]: https://github.com/bijela-gora/automerge-repo-storage-better-sqlite3
