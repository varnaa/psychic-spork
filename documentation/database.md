# Model

#### 1. Books
```json
{
"global_id": {type: "string", required: true}
"name": {type: "string", required: true},
"author_name": {type: "string", required: true},
"instances": [
        {
            "instance_id": {type: "string", required: true},
            "isbn_number": {type: "string", required: true},
            "status": {type: "string", required: true, enum:["Available", "Maintenance", "Loaned", "Reserved"], "default":"Available"},
            "due_back": {type: "date", "default": "Date.now" },
            "loaned_to": {type: "string", required: true, value: "user_id", "default": "None"}
       },
       {
        "instance_id": {type: "string", required: true},
        "isbn_number": {type: "string", required: true},
        "status": {type: "string", required: true, enum:["Available", "Maintenance", "Loaned", "Reserved"], "default":"Available"},
        "due_back": {type: "date", "default": "Date.now" },
        "loaned_to": {type: "string", required: true, value: "user_id", "default": "None"}
       }
   ]
}
```

---

#### 2. Users

```json
{
  "id":{type:"string", required: true},
  "first_name": {type:"string", required: true},
  "last_name": {type:"string", required: true},
  "phone_number": {type: "integer", required: true},
  "address": {type: "string", required: false},
  "user_name":{type:"string", required: true},
  "password": {type: "string", required: true},
  "email": {type: "string", required: true},
  "notifications": [
      {
        "notification_id" : {type:"string", required:true},
        "notification": {type: "string", required: true}
      },
      {
        "notification_id" : {type:"string", required:true},
        "notification": {type: "string", required: true}
      },
    ]
  }
}

```




