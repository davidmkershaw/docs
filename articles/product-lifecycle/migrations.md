---
toc: true
title: Migrations
description: list of all the changes made on auth0 platform that might affect customers
topics:
  - migrations
contenttype:
  - concept
  - reference
usecase:
  - migrate
---

# Migrations

We are actively migrating customers to new behaviors for all **Deprecations** listed below. Please review these carefully to ensure you've taken any necesarry steps to avoid any service disruptions. More information about our Deprecations process can be found on our [Product Lifecycle page](/product-lifecycle).

<table class="table">
  <thead>
    <tr>
      <th style="width: 156px;">Feature/Behavior</th>
      <th style="width: 100px;">Deprecated</th>
      <th style="width: 233px;">End Of Life Date</th>
      <th>Details</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="/users/search/v3/migrate-search-v2-v3">User Search v2</a></td>
      <td>6 June 2018</td>
      <td>30 June 2019</td>
      <td>User Search v2 is being deprecated and you may be required to take action before June 30, 2019. A <a href="/users/search/v3/migrate-search-v2-v3">migration guide</a> is available to walk you through the steps required. Notifications have been and will continue to be sent to customers that need to complete this migration.<br>Useful Resources:<br>
        <a href="/users/search/v3">User Search v3</a><br>
        <a href="/users/search/v3/query-syntax">User Search v3 - Query Syntax</a><br>
        <a href="/best-practices/search-best-practices">User Search Best Practices</a><br>
        <a href="/users/search/v3/migrate-search-v2-v3">User Search v2 to v3 Migration Guide</a><br>
      </td>
    </tr>
    <tr>
      <td><a href="/logs/migrate-logs-v2-v3">Tenant Logs Search v2</a></td>
      <td>21 May 2019</td>
      <td>
        <b>Free</b>: 15 June 2019<br>
        <b>Developer</b>: 20 August 2019<br>
        <b>Developer Pro</b>: 20 August 2019<br>
        <b>Enterprise</b>: 4 November 2019
      </td>
      <td>To provide our customers with the most reliable and scalable solution, Auth0 has deprecated Tenant Logs Search Engine v2 in favor of v3. Auth0 is proactively migrating customers unaffected by this change, while those who are potentially affected are being notified to opt in for v3 during the provided grace period.  See the <a href="/logs/migrate-logs-v2-v3">migration guide</a> for more information.</td>
    </tr>
    <tr>
      <td><a href="/migrations/guides/extensibility-node8">Node.js v4 Extensibility Runtime</a></td>
      <td>17 April 2019</td>
      <td>30 June 2019</td>
      <td>
        The Webtask engine powering Auth0 extensibility points currently utilizes Node 4. Beginning <strong>30 April 2018</strong>, <a href="https://github.com/nodejs/Release#release-schedule">Node.js v4 will no longer be under long-term support (LTS)</a>. This means that critical security fixes will no longer be back-ported to this version. As such, Auth0 will be migrating the Webtask runtime from Node.js v4 to Node.js v8.<br><br>On <strong>17 April 2018</strong> we will make the Node 8 runtime available for extensibility to all public cloud customers. You will be provided a migration switch that allows you to control your environment's migration to the new runtime environment.<br><br>For more information on this migration and the steps you should follow to upgrade your implementation, see <a href="/migrations/guides/extensibility-node8">Migration Guide: Extensibility and Node.js v8</a>.
      </td>
    </tr>
    <tr>
      <td><a href="/migrations/guides/migration-oauthro-oauthtoken">oauth/ro</a></td>
      <td>26 December 2017</td>
      <td>TBD</td>
      <td>
        If you are currently implementing the <a href="/api/authentication#resource-owner">/oauth/ro</a> endpoint your application can be updated to use the <a href="/api/authentication#authorization-code">/oauth/token</a> endpoint. For details on how to make this transition, see the <a href="/migrations/guides/migration-oauthro-oauthtoken">Migration Guide for Resource Owner Password Credentials Exchange</a>.
      </td>
    </tr>
  </tbody>
</table>

If you have any questions, create a ticket in our [Support Center](${env.DOMAIN_URL_SUPPORT}).