Monday, 23 Dec, 2024 11:49:PM

#### Tags: [[pnpm]] [[npm]] [[pnpm store]] [[node_modules]]

##### *This approach is significantly faster than the traditional three-stage installation process of resolving, fetching, and writing all dependencies to `node_modules`.*

## npm:
![[npm-install.png]]
## pnpm:
![[pnpm-add.png]]

- **Dependency resolution**: Identifies dependencies + Fetches to store 
- **Directory structure calculation**: Calculates and constructs the node_modules directory structure
- **Linking dependencies**: Dependencies fetched from the [[pnpm store]], and add [[hard-linked]] to the node_modules.
#### References

- https://pnpm.io/motivation#boosting-installation-speed