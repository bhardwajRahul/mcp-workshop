# OAuth MCP Module

This module demonstrates OAuth 2.0 integration with MCP (Model Context Protocol) servers.

## Implementations

### Dynamic Client Registration (DCR)

The `dcr/` directory contains a complete OAuth 2.0 implementation with Dynamic Client Registration support.

- **[Dynamic Client Registration Implementation](dcr/README.md)**: Full documentation for the DCR-based OAuth flow
- **Key Features**:
  - Multi-provider OAuth (GitHub, GitLab, Gitea)
  - Dynamic client registration endpoint
  - PKCE (Proof Key for Code Exchange) support
  - Flexible storage backends (memory, Redis)

See [dcr/README.md](dcr/README.md) for complete documentation and usage instructions.

## Quick Start

```bash
# Start OAuth server with DCR
cd dcr/oauth-server
go run . -client_id=<your-id> -client_secret=<your-secret>

# Run OAuth client example
cd dcr/oauth-client
go run .
```
