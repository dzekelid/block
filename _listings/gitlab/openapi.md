---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/users/{id}/block:
    put:
      summary: Put Users Block
      description: Block a user. Available only for admins.
      operationId: putV3UsersIdBlock
      x-api-path-slug: v3usersidblock-put
      parameters:
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Block
---