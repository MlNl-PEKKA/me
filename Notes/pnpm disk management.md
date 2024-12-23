Monday, 23 Dec, 2024 11:16:PM

#### Tags: [[pnpm]] [[packages]] [[npm]] [[node_modules]]
#####  *You save a lot of space on your disk proportional to the number of projects and dependencies, and you have a lot faster installations!*

![[pnpm-addressable-store.png]]

- In npm, 100 projects using a dependency, lead to 100 installations of the same dependency.
- In pnpm, all files are saved in a single place on the disk, and dependencies are [[hard-linked]] from that single location.
- For varying version dependencies, only the difference between each version create a new file. 
### References

- https://pnpm.io/motivation#saving-disk-space