# Sample DSL Implementation in Spring Boot App

## Database and Service
### Database Schema Design
- H2 
- Init Script For Reference Data

### Application do the following services
- Available Meeting Rooms
- Book Meeting Room
- Release Meeting Room

## Steps to Run the App
The application should be run at http://localhost:8080/

##### Retrieve Rooms Information
`GET http://localhost:8080/api/rooms`

##### Book Meeting Room
`POST http://localhost:8080/api/booking`

######Request Body

{
	"userInfo": {
		"empId" : "102",
		"email" : "xxx@x.com"
	},
	"roomInfo": {
		"roomId" : "02",
		"timeId" : "102"
	}
}

######Response

{
    "bookingId": "20191114454053381"
}


##### Release Meeting Room
`GET http://localhost:8080/api/release/02/102`


