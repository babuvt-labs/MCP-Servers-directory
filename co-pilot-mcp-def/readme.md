# Configure a Custom Connector

With your MCP server set up, you must configure a custom connector (via **Power Apps** or **Power Automate**) for your MCP server. To carry out this procedure, you need a **schema file** for your MCP server. The schema file is an **OpenAPI specification YAML file** that describes the API of your MCP server.

For guidance on what the specification file should look like, check out some of the provided MCP server schema examples.

---

## Steps

1. **Select** `Agents` in the left navigation.
2. Select your agent from the list of agents.
3. Go to the **Tools** page for your agent.
4. Select **Add a tool**.
5. Select **New tool**.
6. Select **Custom connector**.  
   *You're taken to Power Apps to create a new custom connector.*
7. Select **New custom connector**.
8. Select **Import OpenAPI file**.
9. Navigate to your schema file and select **Import** to import the file.
10. Select **Continue** to complete the setup in Power Apps.  
    *You can read more about the setup process in the Power Apps documentation at [Import the OpenAPI definition](https://learn.microsoft.com/powerapps/maker/connectors/custom-connectors/openapi-connector-overview).*

---

## MCP Server Schema Examples

Here are two sample OpenAPI schema files for MCP servers using fictional data, in YAML format. The samples demonstrate each of the supported transports.  
**You need to fill in the details for your own MCP server.**

---

### Example YAML for Streamable (Recommended)

```yaml
swagger: '2.0'
info:
  title: Contoso
  description: MCP Test Specification, YAML for streamable MCP support in Copilot Studio
  version: 1.0.0
host: contoso.com
basePath: /
schemes:
  - https
paths:
  /mcp:
    post:
      summary: Contoso Lead Management Server
      x-ms-agentic-protocol: mcp-streamable-1.0
      operationId: InvokeMCP
      responses:
        '200':
          description: Success
