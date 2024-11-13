# Feature overview

Olares offers a wide array of features designed to enhance security, ease of use, and development flexibility:

- **Enterprise-grade security**: Secure your self-hosted cloud with simplified network configuration using Tailscale, Headscale, Cloudflare Tunnel, and FRP.
- **Secure and permissionless application ecosystem**: Access nearly 100 free applications in a secure, sandboxed environment. [See what Olares Market has to offer](https://market.olares.xyz/).
- **Unified file system and database**: Support automated scaling, backups, and high availability.
- **Single sign-on**: Log in once to access all applications within Olares with a shared authentication service.
- **AI capabilities**: Manage GPU resources, host AI models locally, and build private knowledge bases with complete privacy.
- **Built-in applications**: Get started with essential pre-installed applications such as Files, Vault, Wise, Profile and Dashboard.
- **Seamless anywhere access**: Access your devices from anywhere using dedicated clients for mobile, desktop, and browsers.
- **Development tools**: Build and port applications easily with comprehensive development tools.

## Feature comparison
:::tip Legend
- 🚀: **Auto**, indicates that the system completes the task automatically.
- ✅: **Yes**, indicates that users without a developer background can complete the setup through the product's UI prompts.
- 🛠️: **Manual Configuration**, indicates that even users with an engineering background need to refer to tutorials to complete the setup.
- ✖️:  **No**, indicates that the feature is not supported.
:::

|                           | Olares                                                                                                     | Synology                                    | TrueNAS                                     | CasaOS                  | Unraid                                        |
|---------------------------|------------------------------------------------------------------------------------------------------------|---------------------------------------------|---------------------------------------------|-------------------------|-----------------------------------------------|
| Multi-node                | ✅                                                                                                          | ✖️                                          | ✅                                           | ✖️                      | ✖️                                            |
| Build-in apps             | ✅ (Rich desktop apps)                                                                                      | ✅ (Rich desktop apps)                       | ✖️ (CLI)                                    | ✅ (Simple desktop apps) | ✅ (Dashboard)                                 |
| Free domain name          | ✅                                                                                                          | ✅                                           | ✖️                                          | ✖️                      | ✖️                                            |
| Auto SSL certificate      | 🚀                                                                                                         | ✅                                           | 🛠️                                         | 🛠️                     | 🛠️                                           |
| Reverse proxy             | 🚀                                                                                                         | ✅                                           | 🛠️                                         | 🛠️                     | 🛠️                                           |
| VPN management            | 🚀                                                                                                         | 🛠️                                         | 🛠️                                         | 🛠️                     | 🛠️                                           |
| Graded app entrance       | 🚀                                                                                                         | 🛠️                                         | 🛠️                                         | 🛠️                     | 🛠️                                           |
| Multi-user management     | ✅ User management <br>🚀 Resource isolation                                                                | ✅ User management<br>🛠️ Resource isolation | ✅ User management<br>🛠️ Resource isolation | ✖️                      | ✅ User management  <br>🛠️ Resource isolation |
| Single login for all apps | 🚀                                                                                                         | ✖️                                          | ✖️                                          | ✖️                      | ✖️                                            |
| Cross-node storage        | 🚀 (Juicefs+<br>MinIO)                                                                                     | ✖️                                          | ✖️                                          | ✖️                      | ✖️                                            |
| Database solution         | 🚀 (Built-in cloud-native solution)                                                                        | 🛠️                                         | 🛠️                                         | 🛠️                     | 🛠️                                           |
| Disaster recovery         | 🚀 (MinIO's [**Erasure Coding**](https://min.io/docs/minio/linux/operations/concepts/erasure-coding.html)) | ✅ RAID                                      | ✅ RAID                                      | ✅ RAID                  | ✅ Unraid Storage                              |
| Backup                    | ✅ App Data  <br>✅ User Data                                                                                | ✅ User Data                                 | ✅ User Data                                 | ✅ User Data             | ✅ User Data                                   |
| App sandboxing            | ✅                                                                                                          | ✖️                                          | ✖️ (K8S's namespace)                        | ✖️                      | ✖️                                            |
| App ecosystem             | ✅ (Official + third-party)                                                                                 | ✅ (Majorly official apps)                   | ✅ (Official + third-party submissions)      | ✅ Majorly official apps | ✅ (Community app market)                      |
| Developer friendly        | ✅ IDE  <br>✅ CLI  <br>✅ SDK  <br>✅ Doc                                                                     | ✅ CLI  <br>✅ SDK  <br>✅ Doc                 | ✅ CLI  <br>✅ Doc                            | ✅ CLI  <br>✅ Doc        | ✅ Doc                                         |
| Local LLM hosting         | 🚀                                                                                                         | 🛠️                                         | 🛠️                                         | 🛠️                     | 🛠️                                           |
| Local LLM app development | 🚀                                                                                                         | 🛠️                                         | 🛠️                                         | 🛠️                     | 🛠️                                           |
| Client platforms          | ✅ Android  <br>✅ iOS  <br>✅ Windows  <br>✅ Mac  <br>✅ Chrome Plugin                                        | ✅ Android  <br>✅ iOS                        | ✖️                                          | ✖️                      | ✖️                                            |
| Client functionality      | ✅ (All-in-one client app)                                                                                  | ✅ (14 separate client apps)                 | ✖️                                          | ✖️                      | ✖️                                            |
