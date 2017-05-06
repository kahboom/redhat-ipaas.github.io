---
title: Users


search: true
---

# Getting Started

A test using the User Guide layout.


## How to Use this Guide

You may have noticed some tabs on the right-hand side. These tabs are there to assist you with the different areas involved in Syndesis, and how they pertain to each model.


# Connections

Everyday in your day-to-day operations you use several web services, such as Salesforce, to complete tasks. In Syndesis, we refer to configured versions of each web service and a specific task, collectively, as a Connection.

An example of a Connection is a "Twitter mention", configured with your Twitter account details. As you'll see later, you use one or more Connections to create an Integration (more on this later).

# Integrations

Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Curabitur blandit tempus porttitor. Vestibulum id ligula porta felis euismod semper.

Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Aenean lacinia bibendum nulla sed consectetur. Maecenas faucibus mollis interdum. Cras justo odio, dapibus ac facilisis in, egestas eget quam.

# Templates

> To authorize, use this code:

```c
#require 'kittn'
#
#api = Kittn::APIClient.authorize!('meowmeowmeow')
```

```typescript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
```

> Make sure to replace `meowmeowmeow` with your API key.

Kittn uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>

# Admin

## Test

```c
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get
```

```typescript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let kittens = api.kittens.get();
```

> The above command returns JSON structured like this:

```c
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all kittens.

# Feedback

We are always interested in your feedback! Don't hesitate to shoot us an email to ipaas-dev@redhat.com with any questions, bug reports, or feedback.


### Test

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Test

```c
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get(2)
```

```typescript
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get(2)
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### Test

`GET http://example.com/kittens/<ID>`

### Test

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve

