# ![LOGO](logo.png) IllumiDesk **flow**ground Connector

## Description

A generated **flow**ground connector for the IllumiDesk API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/illumidesk.com/1.0/swagger.json<br/>
Generated at: 2019-05-07T17:42:24+03:00

## API Description



## Authorization

Supported authorization schemes:
- API Key
## Actions

### Create JSON Web Token (JWT)

*Tags:* `auth`

### Refresh a JSON Web Token (JWT)

> Obtains a new JSON Web Token using existing user credentials.

*Tags:* `auth`

### Validate JSON Web Token (JWT)

> Checks veraciy of token.

*Tags:* `auth`

### oauth_login

*Tags:* `auth`

#### Input Parameters
* `provider` - _required_ - OAuth2 provider
    Possible values: github, google, slack.

### Register a user

> User registration requires confirming email address to activate user.

*Tags:* `auth`

### A convenience endpoint that is equivalent to GET /v1/users/profiles/<my user id>/

*Tags:* `users`

### Retrieve available server sizes

*Tags:* `servers`

#### Input Parameters
* `limit` - _optional_ - Set limit when retrieving items.
* `offset` - _optional_ - Offset when retrieving items.
* `ordering` - _optional_ - Set order when retrieving items.

### Create a new server size item

> Only super users with on-premises version have acceess to this endpoint.

*Tags:* `servers`

### Delete a server size by id

> Only super users with on-premises version have acceess to this endpoint.

*Tags:* `servers`

#### Input Parameters
* `size` - _required_ - Server size unique identifier expressed as UUID or name.

### Get a server size by id

*Tags:* `servers`

#### Input Parameters
* `size` - _required_ - Server size unique identifier expressed as UUID or name.

### Update a server size by id

> Only super users with on-premises version have acceess to this endpoint.

*Tags:* `servers`

#### Input Parameters
* `size` - _required_ - Server size unique identifier expressed as UUID or name.

### Replace a server size by id

> Only super users with on-premises version have acceess to this endpoint.

*Tags:* `servers`

#### Input Parameters
* `size` - _required_ - Server size unique identifier expressed as UUID or name.

### Get teams

*Tags:* `teams`

#### Input Parameters
* `limit` - _optional_ - Limit when getting data.
* `offset` - _optional_ - Offset when getting data.

### Create a new team

*Tags:* `teams`

### Delete a team

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.

### Get a team

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.

### Update a team

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.

### Replace a team

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.

### Get team invoices

*Tags:* `teams` `billing`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `limit` - _optional_ - Limit when getting items.
* `offset` - _optional_ - Offset when getting items.

### Get an invoice

*Tags:* `teams` `billing`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `id` - _required_ - Invoice unique identifier expressed as UUID.

### Get team invoice items for a given invoice.

*Tags:* `teams` `billing`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `invoice_id` - _required_ - Invoice id, expressed as UUID.
* `limit` - _optional_ - Limit when getting items.
* `offset` - _optional_ - Offset when getting items.
* `ordering` - _optional_ - Ordering when getting items.

### Get a specific team InvoiceItem.

*Tags:* `teams` `billing`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `invoice_id` - _required_ - Invoice id, expressed as UUID.
* `id` - _required_ - InvoiceItem id, expressed as UUID.

### Get active team subscriptons

*Tags:* `teams` `billing`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `limit` - _optional_ - Limit when getting items.
* `offset` - _optional_ - Offset when getting items.
* `ordering` - _optional_ - Ordering when getting items.

### Create a new team subscription

*Tags:* `teams` `billing`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.

### Delete a subscription

*Tags:* `teams` `billing`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `id` - _required_ - Subscription unique identifier expressed as UUID.

### Get team subscriptions

*Tags:* `teams` `billing`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `id` - _required_ - Unique identifier expressed as UUID.

### Get team groups

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `limit` - _optional_ - Limit when getting data.
* `offset` - _optional_ - Offset when getting data.

### Delete team group

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `group` - _required_ - Group unique identifier expressed as UUID or name.

### Get team group

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `group` - _required_ - Group unique identifier expressed as UUID or name.

### Patch team group

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `group` - _required_ - Group unique identifier expressed as UUID or name.

### Patch team group

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `group` - _required_ - Group unique identifier expressed as UUID or name.

### Add user to group

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `group` - _required_ - Group unique identifier expressed as UUID or name.

### User removed from group

*Tags:* `teams`

#### Input Parameters
* `team` - _required_ - Team unique identifier expressed as UUID or name.
* `group` - _required_ - Group unique identifier expressed as UUID or name.

### Get user list

*Tags:* `users`

#### Input Parameters
* `limit` - _optional_ - Limit user list.
* `offset` - _optional_ - Offset when getting users.
* `username` - _optional_ - User username.
* `email` - _optional_ - User email.
* `ordering` - _optional_ - Ordering when getting users.

### Create new user

> Only admin users can create new users. New users have active status by default.

*Tags:* `users`

### Delete a user

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User identifier expressed as UUID or username.

### Retrieve a user

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - Unique identifier expressed as UUID or username.

### Update a user

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Retrieve account's API key

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Delete avatar

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Retrieve user's avatar

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User unique identifier expressed as UUIDor username.

### Update a project file

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Add user avatar

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Retrieve account email addresses

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User unique identifier as expressed as UUID or username.
* `limit` - _optional_ - Limite when getting email list.
* `offset` - _optional_ - Offset when getting email list.
* `ordering` - _optional_ - Ordering when getting email list.

### Create an email address

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Delete an email address

*Tags:* `users`

#### Input Parameters
* `email_id` - _required_ - Email unique identifier expressed as UUID.
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Retrieve a user's email addresses

*Tags:* `users`

#### Input Parameters
* `email_id` - _required_ - Email unique identifier expressed as UUID.
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Update an email address

*Tags:* `users`

#### Input Parameters
* `email_id` - _required_ - Email unique identifier expressed as UUID.
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Replace an email address

*Tags:* `users`

#### Input Parameters
* `email_id` - _required_ - Email unique identifier expressed as UUID.
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Retrieve an SSH key

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Recreate an SSH key

*Tags:* `users`

#### Input Parameters
* `user` - _required_ - User unique identifier expressed as UUID or username.

### Get credit cards

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Set limit when retrieving credit or debit cards.
* `offset` - _optional_ - Set offset when retriving cards.
* `ordering` - _optional_ - Order when retrieving cards.

### Create new credit card

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.

### Delete a credit card

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Card unique identifier expressed as UUID.

### Get credit card by id

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `id` - _required_ - User unique identifier expressed as UUID.

### Update a credit card

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Card unique identifier.

### Replace a credit card

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `id` - _required_

### Get invoices

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Limit when getting items.
* `offset` - _optional_ - Offset when getting items.
* `ordering` - _optional_ - Ordering when getting items.

### Get an invoice

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Invoice unique identifier expressed as UUID.

### Get invoice items for a given invoice.

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `invoice_id` - _required_ - Invoice id, expressed as UUID.
* `limit` - _optional_ - Limit when getting items.
* `offset` - _optional_ - Offset when getting items.
* `ordering` - _optional_ - Ordering when getting items.

### Get a specific InvoiceItem.

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `invoice_id` - _required_ - Invoice id, expressed as UUID.
* `id` - _required_ - InvoiceItem id, expressed as UUID.

### Get billing plans

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Limit when getting items.
* `offset` - _optional_ - Offset when getting items.
* `ordering` - _optional_ - Ordering when getting items.

### Get a billing plan

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Plan unique identifier expressed as UUID.

### Get active subscriptons

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Limit when getting items.
* `offset` - _optional_ - Offset when getting items.
* `ordering` - _optional_ - Ordering when getting items.

### Create a new subscription

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.

### Delete a subscription

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Subscription unique identifier expressed as UUID.

### Get a subscriptions

*Tags:* `billing`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Unique identifier expressed as UUID.

### Get notifications of all types and entities for the authenticated user.

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team data.
* `limit` - _optional_ - Limit when getting items.
* `offset` - _optional_ - Offset when getting items.
* `ordering` - _optional_ - Ordering when getting items.
* `read` - _optional_ - When true, get only read notifications. When false, get only unread notifications. Default behavior is to return both read and unread.

### Mark a list of notifications as either read or unread.

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team name.

### Get notifications of all types and entities for the authenticated user.

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team data.
* `limit` - _optional_ - Limit when getting items.
* `offset` - _optional_ - Offset when getting items.
* `ordering` - _optional_ - Ordering when getting items.
* `entity` - _required_ - Entity to filter notifications by.
    Possible values: billing.
* `read` - _optional_ - When true, get only read notifications. When false, get only unread notifications. Default behavior is to return both read and unread.

### Mark a list of notifications as either read or unread.

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `entity` - _required_ - Entity to filter notifications by.
    Possible values: billing.

### Retrieve global notification settings for the authenticated user

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team data.

### Modify global notification settings.

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team name.

### Create global notification settings

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team name.

### Retrieve global notification settings for the authenticated user

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team data.
* `entity` - _required_ - Entity whose settings should be retrieved.
    Possible values: billing.

### Modify global notification settings.

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `entity` - _required_ - Entity whose settings should be retrieved.
    Possible values: billing.

### Create global notification settings

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `entity` - _required_ - Entity whose settings should be retrieved.
    Possible values: billing.

### Retrieve a specific notification.

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team data.
* `notification_id` - _required_ - Notification UUID.

### Mark a specific notification as either read or unread.

*Tags:* `notifications`

#### Input Parameters
* `namespace` - _required_ - User or team data.
* `notification_id` - _required_ - Notification UUID.

### Retrieve oauth applications

*Tags:* `oauth`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Set limit when retrieving items.
* `offset` - _optional_ - Offset when retrieving items.
* `ordering` - _optional_ - Set order when retrieving items.

### Create a new OAuth2 application

*Tags:* `oauth`

#### Input Parameters
* `namespace` - _required_ - User or team name.

### Delete an application by id

*Tags:* `oauth`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `application` - _required_ - Application unique identifier expressed as UUID or name.

### Get an application by id

*Tags:* `oauth`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `application` - _required_ - Application unique identifier expressed as UUID or name.

### Update an application by id

*Tags:* `oauth`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `application` - _required_ - Application unique identifier expressed as UUID or name.

### Replace an application by id

*Tags:* `oauth`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `application` - _required_ - Application unique identifier expressed as UUID or name.

### Get available projects

*Tags:* `projects`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Limit when getting data.
* `offset` - _optional_ - Offset when getting data.
* `private` - _optional_ - Private project or public project.
* `name` - _optional_ - Project name.
* `ordering` - _optional_ - Ordering when getting projects.

### Create a new project

*Tags:* `projects`

#### Input Parameters
* `namespace` - _required_ - User or team name.

### Check if you are able to copy a project to your account.

*Tags:* `projects`

#### Input Parameters
* `namespace` - _required_ - User or team name.

### Copy a project to your own account.

*Tags:* `projects`

#### Input Parameters
* `namespace` - _required_ - User or team name.

### Delete a project

*Tags:* `projects`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.

### Get a project

*Tags:* `projects`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.

### Update a project

*Tags:* `projects`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.

### Replace a project

*Tags:* `projects`

#### Input Parameters
* `namespace` - _required_ - User or team namespace.
* `project` - _required_ - Project unique identifier expressed as UUID or name.

### Get project collaborators

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Limit when retrieving items.
* `offset` - _optional_ - Offset when retrieving items.
* `ordering` - _optional_ - Ordering when retrieving items.

### Create project collaborators

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.

### Delete a project collaborator

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier.
* `namespace` - _required_ - User or team name.
* `collaborator` - _required_ - Collaborator unique identifier.

### Get a project collaborator

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier.
* `namespace` - _required_ - User or team name.
* `collaborator` - _required_ - Collaborator unique identifier expressed as UUID or name.

### Update project collaborator

*Tags:* `projects`

#### Input Parameters
* `project` - _required_
* `namespace` - _required_ - User or team name.
* `collaborator` - _required_

### Retrieve deployments

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Limit results when getting deployment list.
* `offset` - _optional_ - Offset results when getting deployment list.
* `name` - _optional_ - Server name.
* `ordering` - _optional_ - Ordering option when getting deployment list.

### Create a new deployment

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifer expressed as UUID or name.
* `namespace` - _required_ - User or team name.

### Delete a deployment

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier.
* `namespace` - _required_ - User or team name.
* `deployment` - _required_ - User unique identifier.

### Retrieve a deployment

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `deployment` - _required_ - Deployment unique identifier expressed as UUID or name.

### Update a deployment

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `deployment` - _required_ - Deployment unique identifier expressed as UUID or name.

### Replace a deployment

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `deployment` - _required_ - Deployment unique identifier expressed as UUID or name.

### Deploy an existing model

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `deployment` - _required_ - Deployment unique identifier expressed as UUID or name.

### Get project files

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Unique identifier for project file expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Limit when getting project file list.
* `offset` - _optional_ - Offset when getting project file list.
* `ordering` - _optional_ - Ordering of list values when getting project file list.
* `filename` - _optional_ - Exact file name, relative to the project root. If no such file is found, an empty list will be returned.
* `content` - _optional_ - Determines whether or not content is returned as base64. Defaults to false.

### Create project files

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier.
* `namespace` - _required_ - User or team name.

### Delete a project file

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifer.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - File unique identifier.

### Get a project file

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifer.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - File unique identifier.
* `content` - _optional_ - Determines whether or not content is returned as base64. Defaults to false.

### Update a project file

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifer.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - File unique identifier.

### Replace a project file

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifer.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - File unique identifier.

### Retrieve servers

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Limit results when getting server list.
* `offset` - _optional_ - Offset results when getting server list.
* `name` - _optional_ - Server name.
* `ordering` - _optional_ - Ordering option when getting server list.

### Create a new server

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifer expressed as UUID or name.
* `namespace` - _required_ - User or team name.

### Retrieve server statuses

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.

### Delete a server

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier.
* `namespace` - _required_ - User or team name.
* `server` - _required_ - User unique identifier.

### Retrieve a server

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `server` - _required_ - Server unique identifier expressed as UUID or name.

### Update a server

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `server` - _required_ - Server unique identifier expressed as UUID or name.

### Replace a server

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `server` - _required_ - Server unique identifier expressed as UUID or name.

### Get server API key

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `server` - _required_ - Server unique identifier expressed as UUID or name.

### Server api key validation

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `server` - _required_ - Server unique identifier expressed as UUID or name.

### Create a new server's run statistics

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.

### Delete a server's statistics

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Server run statistics unique identifier expressed as UUID.

### Retrieve statistics for a server

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Run statistics unique identifier expressed as UUID.

### Update a server's statistics

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Server run statistics unique identifier expressed as UUID.

### Replace a server's statistics

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Server run statistics expressed as UUID.

### Get SSH Tunnels associated to a server

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `limit` - _optional_ - Limit retrieved items.
* `offset` - _optional_ - Offset retrieved items.
* `ordering` - _optional_ - Order retrieved items.

### Create SSH Tunnel associated to a server

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.

### Delete an SSH Tunnel associated to a server

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `tunnel` - _required_ - SSH tunnel unique identifier expressed as UUID or name.

### Get an SSH Tunnel associated to a server

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `tunnel` - _required_ - SSH tunnel unique identifier expressed as UUID or name.

### Update an SSH Tunnel associated to a server

*Tags:* `projects`

#### Input Parameters
* `server` - _required_
* `project` - _required_
* `namespace` - _required_ - User or team name.
* `tunnel` - _required_

### Replace SSH Tunnel associated to a server

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `tunnel` - _required_ - SSH tunnel unique identifier expressed as UUID or name.

### Start a server

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `server` - _required_ - Server unique identifier expressed as UUID or name.

### Delete a server's statistics

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Stats unique identifier expressed as UUID.

### Retrieve a server's statistics

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Server statistics unique identifier expressed as UUID.

### Update a server's statistics

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Server statistics unique identifier expressed as UUID.

### Replace a server's statistics

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `id` - _required_ - Server statistics unique identifier expressed as UUID.

### Stop a server

*Tags:* `projects`

#### Input Parameters
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `server` - _required_ - Server unique identifier expressed as UUID or name.

### Retrieve server triggers

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `name` - _optional_ - Trigger name.
* `limit` - _optional_ - Limit when getting triggers.
* `offset` - _optional_ - Offset when getting triggers.
* `ordering` - _optional_ - Ordering when getting triggers.

### Create a new server trigger

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.

### Delete a server trigger

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `trigger` - _required_ - Trigger identifier expressed as UUID or name.

### Get a server trigger

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `trigger` - _required_ - Trigger unique identifier.

### Update a server trigger

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `trigger` - _required_ - Trigger identifier expressed as UUID or name.

### Replace a server trigger

*Tags:* `projects`

#### Input Parameters
* `server` - _required_ - Server unique identifier expressed as UUID or name.
* `project` - _required_ - Project unique identifier expressed as UUID or name.
* `namespace` - _required_ - User or team name.
* `trigger` - _required_ - Trigger unique identifier.

### Get a search results

*Tags:* `search`

#### Input Parameters
* `namespace` - _required_ - User or team name.
* `q` - _required_ - Search string.
* `type` - _optional_ - Limit results to specific types.
    Possible values: users, projects, servers.
* `limit` - _optional_ - Limit data when getting items.
* `offset` - _optional_ - Offset data when getting items.

## License

**flow**ground :- Telekom iPaaS / illumidesk-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
