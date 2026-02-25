aerolites-bookings-backend/
├── mocks/
│ └── mocks.go
|
├── app/
│ ├── server/
│ │ └── start.go
| |
│ ├── booking/
| | |
│ │ ├── constants/
│ │ │ └── App_constants
| | |
│ │ ├── controller/
│ │ │ ├── booking_controller
│ │ │ ├── revenue_controller
│ │ │ ├── shows_controller
│ │ │ └── User_controller
| | |
│ │ ├── database/
│ │ │ ├── common/
│ │ │ │ └── Base_db
│ │ │ ├── connection/
│ │ │ │ └── connection.go
│ │ │ └── seed/
│ │ │ └── dataseeder.go
| | |
│ │ ├── dto/
│ │ │ ├── request/
│ │ │ │ ├── Booking_request
│ │ │ │ └── booking_request_Test
│ │ │ └── response/
│ │ │ ├── Booking_confirmation_response
│ │ │ └── Show_responses
| | |
│ │ ├── Model/
│ │ │ ├── booking.go
│ │ │ ├── customer.go
│ │ │ ├── movie.go
│ │ │ ├── show.go
│ │ │ ├── slot.go
│ │ │ └── user.go
| | |
│ │ └── repository/
│ │ ├── booking_Repository
│ │ ├── Customer_repository
│ │ ├── show_repository
│ │ └── User_repository
| |
│ ├── service/
│ │ ├── Booking_service
│ │ ├── Revenue_service
│ │ ├── Shows_service
│ │ └── user_Service
| |
│ ├── common/
│ │ └── logger/
│ │ └── logger.go
| |
│ ├── middleware/
│ │ ├── cors/
│ │ │ └── cors.go
│ │ ├── security/
│ │ │ └── basic_Auth
│ │ ├── validator/
│ │ │ └── Dto_validation_handler
│ │ └── Dto_validator
│ └── config/
├── docs/
├── error/
├── infrastructure/
├── integration_test/
├── migration/
├── Movieservice/
├── movie_gateway/
│ ├── Movie_gateway
│ └── Movie_service
├── out/
├── scripts/
├── .gitignore
├── .tailsmanrc
├── Appspec.yml
├── aws_check_cluster_Status
├── Buildspec
├── Creds_input_file
├── Deploy
├── deploy.sh
├── Docker_database_setup.md
├── Docker-compose-local
├── docker-compose.ci.yml
├── Docker-compose
├── Dockerfile
├── Dockerfile-migration
├── Ecs-registry-creds
├── Env
├── Go.mod
├── Go.sum
├── healthcheck.sh
├── main.go
├── Makerfile
├── promote.sh
├── readme.md
├── Run-backend-local
├── todo.md
└── verify.sh
