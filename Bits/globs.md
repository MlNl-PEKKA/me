Tuesday, 24 Dec, 2024 12:07:AM

##### *A pattern to match files. Similar to regex*

- *`*`*
	-  Matches zero or more characters, on the same directory level
	- Pattern: `src/*.ts`
	- Matches: `src/index.ts`, `src/foo.ts`
	- Does NOT match: `src/subdir/foo.ts`
	`
- *`**`*
	- Matches zero or more characters, recursively
	-  Pattern: `src/**/*.ts`
	- Matches: `src/index.ts`, `src/foo.ts`, `src/subdir/foo.ts`
	
- **`?`**
    - Matches exactly one character.
    - Pattern: `src/file?.ts`
    - Matches: `src/file1.ts`, `src/fileA.ts`
    - Does NOT match: `src/file123.ts`
    
- **`[abc]` (Character Set)**:
    - Matches one character from the set.
    - Pattern: `src/file[12].ts`
    - Matches: `src/file1.ts`, `src/file2.ts`
    - Does NOT match: `src/file3.ts
     `
- **`!` (Negation)**:
    - Excludes files that match the pattern.
    - Pattern: `!src/*.test.ts`
    - Excludes: `src/foo.test.ts`, `src/bar.test.ts`