# Mirky API

---

<aside>
👉 api.mirky.app

</aside>

---

## Endpoints

```json
GET /v1/

{
	"message":"poop"
}
```

### Auth Routes

```json
POST /v1/auth/annonSession

{
	"sessionId":string
}
```

```json
POST /v1/auth/signup

{
	"message":"User created, session replaced",
	"sessionId":string
}
```

```json
POST /v1/auth/login

{
	"message":"User logged in, session replaced",
	"sessionId":string
}
```

### Property Routes

```json
POST /v1/property/create

{
	"message":"Property created",
	"property": {
		"propUid":string,
		"propName":string,
		"comapnyName":string,
		"website":string,
		"industry":string,
		"companySize":string,
		"createdAt":Date,
		"updatedAt":Date
	}
}
		
```

```json
POST /v1/property/fetch-users-props

{
	"properties":Array
}
```