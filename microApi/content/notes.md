
---
weight: 11
title: notes
---

# notes


## Notes.Create

```go
package main

import (
  "github.com/micro/clients/go/client"
  notes_proto "github.com/micro/services/notes/proto"
)

func main() {
  c := client.NewClient(nil)

  req := notes_proto.CreateNoteRequest{}
  rsp := notes_proto.CreateNoteResponse{}

  if err := c.Call("go.micro.srv.notes", "Notes.Create", req, &rsp); err != nil {
    fmt.Println(err)
    return
  }
  fmt.Println(rsp)
}
```

```javascript
// To install "npm install --save @microhq/ng-client"

import { Component, OnInit } from "@angular/core";
import { ClientService } from "@microhq/ng-client";

@Component({
  selector: "app-example",
  templateUrl: "./example.component.html",
  styleUrls: ["./example.component.css"]
})
export class ExampleComponent implements OnInit {
  constructor(private mc: ClientService) {}

  ngOnInit() {
    this.mc
      .call("go.micro.srv.notes", "Notes.Create", {})
      .then((response: any) => {
        console.log(response)
      });
  }
}
```




### Request Parameters

Name |  Type | Description
--------- | --------- | ---------
note | Note | 


### Response Parameters

Name |  Type | Description
--------- | --------- | ---------
note | Note | 



<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Notes.Delete

```go
package main

import (
  "github.com/micro/clients/go/client"
  notes_proto "github.com/micro/services/notes/proto"
)

func main() {
  c := client.NewClient(nil)

  req := notes_proto.DeleteNoteRequest{}
  rsp := notes_proto.DeleteNoteResponse{}

  if err := c.Call("go.micro.srv.notes", "Notes.Delete", req, &rsp); err != nil {
    fmt.Println(err)
    return
  }
  fmt.Println(rsp)
}
```

```javascript
// To install "npm install --save @microhq/ng-client"

import { Component, OnInit } from "@angular/core";
import { ClientService } from "@microhq/ng-client";

@Component({
  selector: "app-example",
  templateUrl: "./example.component.html",
  styleUrls: ["./example.component.css"]
})
export class ExampleComponent implements OnInit {
  constructor(private mc: ClientService) {}

  ngOnInit() {
    this.mc
      .call("go.micro.srv.notes", "Notes.Delete", {})
      .then((response: any) => {
        console.log(response)
      });
  }
}
```




### Request Parameters

Name |  Type | Description
--------- | --------- | ---------
note | Note | 


### Response Parameters

Name |  Type | Description
--------- | --------- | ---------



<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Notes.List

```go
package main

import (
  "github.com/micro/clients/go/client"
  notes_proto "github.com/micro/services/notes/proto"
)

func main() {
  c := client.NewClient(nil)

  req := notes_proto.ListNotesRequest{}
  rsp := notes_proto.ListNotesResponse{}

  if err := c.Call("go.micro.srv.notes", "Notes.List", req, &rsp); err != nil {
    fmt.Println(err)
    return
  }
  fmt.Println(rsp)
}
```

```javascript
// To install "npm install --save @microhq/ng-client"

import { Component, OnInit } from "@angular/core";
import { ClientService } from "@microhq/ng-client";

@Component({
  selector: "app-example",
  templateUrl: "./example.component.html",
  styleUrls: ["./example.component.css"]
})
export class ExampleComponent implements OnInit {
  constructor(private mc: ClientService) {}

  ngOnInit() {
    this.mc
      .call("go.micro.srv.notes", "Notes.List", {})
      .then((response: any) => {
        console.log(response)
      });
  }
}
```




### Request Parameters

Name |  Type | Description
--------- | --------- | ---------


### Response Parameters

Name |  Type | Description
--------- | --------- | ---------
notes | Note | 



<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Notes.Update

```go
package main

import (
  "github.com/micro/clients/go/client"
  notes_proto "github.com/micro/services/notes/proto"
)

func main() {
  c := client.NewClient(nil)

  req := notes_proto.UpdateNoteRequest{}
  rsp := notes_proto.UpdateNoteResponse{}

  if err := c.Call("go.micro.srv.notes", "Notes.Update", req, &rsp); err != nil {
    fmt.Println(err)
    return
  }
  fmt.Println(rsp)
}
```

```javascript
// To install "npm install --save @microhq/ng-client"

import { Component, OnInit } from "@angular/core";
import { ClientService } from "@microhq/ng-client";

@Component({
  selector: "app-example",
  templateUrl: "./example.component.html",
  styleUrls: ["./example.component.css"]
})
export class ExampleComponent implements OnInit {
  constructor(private mc: ClientService) {}

  ngOnInit() {
    this.mc
      .call("go.micro.srv.notes", "Notes.Update", {})
      .then((response: any) => {
        console.log(response)
      });
  }
}
```




### Request Parameters

Name |  Type | Description
--------- | --------- | ---------
note | Note | 


### Response Parameters

Name |  Type | Description
--------- | --------- | ---------



<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Notes.UpdateStream

```go
package main

import (
  "github.com/micro/clients/go/client"
  notes_proto "github.com/micro/services/notes/proto"
)

func main() {
  c := client.NewClient(nil)

  req := notes_proto.UpdateNoteRequest{}
  rsp := notes_proto.UpdateNoteResponse{}

  if err := c.Call("go.micro.srv.notes", "Notes.UpdateStream", req, &rsp); err != nil {
    fmt.Println(err)
    return
  }
  fmt.Println(rsp)
}
```

```javascript
// To install "npm install --save @microhq/ng-client"

import { Component, OnInit } from "@angular/core";
import { ClientService } from "@microhq/ng-client";

@Component({
  selector: "app-example",
  templateUrl: "./example.component.html",
  styleUrls: ["./example.component.css"]
})
export class ExampleComponent implements OnInit {
  constructor(private mc: ClientService) {}

  ngOnInit() {
    this.mc
      .call("go.micro.srv.notes", "Notes.UpdateStream", {})
      .then((response: any) => {
        console.log(response)
      });
  }
}
```




### Request Parameters

Name |  Type | Description
--------- | --------- | ---------
note | Note | 


### Response Parameters

Name |  Type | Description
--------- | --------- | ---------



<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

