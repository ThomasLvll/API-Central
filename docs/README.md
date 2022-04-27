<!-- PROJECT HEADER -->
<div align="center">
  <!-- <img src="docs/img/logo.png" alt="Logo" width="80" height="80">
  --><h3 align="center">API Central</h3>

  <p align="center">
    <a href="https://github.com/ThomasLvll/API-Central"><strong>» Main Page</strong></a>
    <br />
    <h1>Documentation</h1>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#api">API</a>
    </li>
    <li>
      <a href="#permissions">Permissions</a>
    </li>
  </ol>
</details>



## API

[Definition](api-definition.yaml) and [documentation](api-documentation/) of API have been done using [Postman](https://www.postman.com/).
They follow [OpenAPI 3.0.3 specification](https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.0.3.md).

<p align="right">(<a href="#top">back to top</a>)</p>



## Permissions

To allow only certain users to manipulate particular data within API Central and served APIs, permissions can be assigned to users and API tokens.

A permission has the form:

```
context:right
```

`context` is the scope on which the permission is assigned, and `right` is the type of permission. For example, `central:create-api` allows user to add an API within API Central.

Both `context` and `right` can be replaced with the `*` wildcard, giving user a permission within all the contexts, and/or all the permissions within a context.

___Warning: giving full permissions to a user is rarely the best solution, so the `*` wildcard should be used with caution.___

<p align="right">(<a href="#top">back to top</a>)</p>
