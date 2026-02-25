skyfox-booking-backend/
| movie-service/
| ├── movie-gateway/
| │ ├── main.go
| │ ├── routes.go
| │ ├── middleware/
| │ ├── auth_middleware.go
| │ ├── rate_limiter.go
| │ └── cors.go
| └── config/
| └── gateway_config.go
│
├── app/
│ └── server/
│ └── start.go
│
├── internal/
│ ├── auth/
│ │ ├── controller/
│ │ │ ├── auth_controller.go
│ │ │ ├── signup_controller.go
│ │ │ ├── login_controller.go
│ │ │ ├── email_verification_controller.go
│ │ │ ├── phone_verification_controller.go
│ │ │ ├── captcha_controller.go
│ │ │ ├── reset_password_controller.go
│ │ │ └── change_password_controller.go
│ │ ├── service/
│ │ │ ├── auth_service.go
│ │ │ ├── otp_service.go
| | | ├── email-verification-service.go
│ │ │ ├── captcha_service.go
│ │ │ └── password_service.go
│ │ ├── repository/
│ │ │ ├── auth_repository.go
│ │ │ └── otp_repository.go
│ │ ├── domains/
│ │ │ ├── verification.go
│ │ │ └── otp.go
│ │ └── dto/
│ │ ├── signup_request.go
│ │ ├── login_request.go
│ │ ├── reset_password_request.go
│ │ ├── change_password_request.go
│ │ ├── email_verification_request.go
│ │ └── phone_verification_request.go
│ │
│ ├── user/
│ │ ├── controller/
│ │ │ ├── admin_profile_controller.go
│ │ │ ├── customer_profile_controller.go
│ │ │ ├── update_profile_controller.go
│ │ │ ├── avatar_controller.go
│ │ │ └── file_upload_controller.go
│ │ ├── service/
│ │ │ ├── user_service.go
│ │ │ ├── profile_service.go
│ │ │ └── avatar_service.go
│ │ ├── repository/
│ │ │ └── user_repository.go
│ │ ├── domains/
│ │ │ ├── user.go
│ │ │ ├── avatar.go
│ │ │ └── profile_image.go
│ │ └── dto/
│ │ ├── user_profile_response.go
│ │ └── update_profile_request.go
│ │
│ ├── show/
│ │ ├── controller/
│ │ │ ├── show_schedule_controller.go
│ │ │ ├── slot_controller.go
│ │ │ └── screen_controller.go
│ │ ├── service/
│ │ │ ├── show_service.go
│ │ │ ├── slot_service.go
│ │ │ └── validation_service.go
│ │ ├── repository/
│ │ │ └── show_repository.go
│ │ ├── domains/
│ │ │ ├── show.go
│ │ │ ├── slot.go
│ │ │ └── screen.go
│ │ └── dto/
│ │ └── show_schedule_request.go
│ │
│ ├── theatre/
│ │ ├── controller/
│ │ │ └── seat_controller.go
│ │ ├── service/
│ │ │ ├── seat_service.go
│ │ │ └── seat_map_service.go
│ │ ├── repository/
│ │ │ └── seat_repository.go
│ │ ├── domains/
│ │ │ ├── seat.go
│ │ │ └── seat_type.go
│ │ └── dto/
│ │ ├── seat_map_response.go
│ │ └── seat_selection_request.go
│ │
│ ├── booking/
│ │ ├── controller/
│ │ │ ├── booking_controller.go
│ │ │ └── checkin_controller.go
│ │ ├── service/
│ │ │ ├── booking_service.go
│ │ │ ├── seat_locking_service.go
│ │ │ └── checkin_service.go
│ │ ├── repository/
│ │ │ ├── booking_repository.go
│ │ │ └── checkin_repository.go
│ │ ├── domains/
│ │ │ ├── booking.go
│ │ │ └── checkin.go
│ │ └── dto/
│ │ ├── booking_request.go
│ │ └── booking_confirmation_response.go
│ │
│ ├── payment/
│ │ ├── controller/
│ │ │ └── payment_controller.go
│ │ ├── service/
│ │ │ └── payment_service.go
│ │ ├── repository/
│ │ │ └── payment_repository.go
│ │ ├── domains/
│ │ │ ├── payment.go
│ │ │ └── transaction.go
│ │ └── dto/
│ │ └── payment_request.go
│ │
│ ├── revenue/
│ │ ├── controller/
│ │ │ ├── revenue_movie_controller.go
│ │ │ ├── revenue_timeframe_controller.go
│ │ │ ├── revenue_showtime_controller.go
│ │ │ └── csv_download_controller.go
│ │ ├── service/
│ │ │ └── revenue_service.go
│ │ ├── repository/
│ │ │ └── revenue_repository.go
│ │ └── dto/
│ │ └── revenue_dashboard_response.go
│ │
│ ├── notification/
│ │ ├── controller/
│ │ │ └── notification_controller.go
│ │ ├── service/
│ │ │ ├── email_service.go
│ │ │ ├── sms_service.go
│ │ │ ├── qr_service.go
│ │ │ └── push_service.go
│ │ └── domains/
│ │ └── qr_ticket.go
│ │
│ └── shared/
│ ├── database/
│ │ ├── connection.go
│ │ └── base.go
│ ├── logger/
│ │ └── logger.go
│ ├── middleware/
│ │ ├── jwt.go
│ │ ├── rbac.go
│ │ ├── rate_limiter.go
│ │ └── cors.go
│ ├── validator/
│ │ └── dto_validator.go
│ │ ├── router/
│ │ │ ├── router.go <-- central route setup
│ │ │ ├── public_routes.go
│ │ │ ├── protected_routes.go
│ │ │ ├── admin_routes.go
│ │ │ └── staff_routes.go
│ │
│ └── config/
│ ├── app_config.go
│ ├── payment_config.go
│ ├── captcha_config.go
│ └── storage_config.go
│
├── infrastructure/
│ ├── captcha/
│ │ └── captcha_client.go
│ ├── imdb/
│ │ └── imdb_client.go
│ ├── payment_gateway/
│ │ └── gateway_client.go
│ ├── storage/
│ │ └── s3_storage.go
│ ├── email/
│ │ └── email_sender.go
│ └── sms/
│ └── sms_sender.go
│
├── migrations/
│ ├── user.sql
│ ├── show.sql
│ ├── seat.sql
│ ├── booking.sql
│ ├── payment.sql
│ └── revenue.sql
│
├── tests/
│ ├── integration/
│ └── unit/
│
├── docker/
│ ├── Dockerfile
│ └── docker-compose.yml
│
├── scripts/
├── docs/
├── main.go
└── go.mod

MovieService/ (Separate Microservice)
├── cmd/
│ └── main.go
├── controller/
│ ├── movie_controller.go
│ └── trailer_controller.go
├── service/
│ └── movie_service.go
├── repository/
│ └── movie_repository.go
├── domains/
│ └── movie.go
├── dto/
│ ├── imdb_rating_response.go
│ └── trailer_response.go
├── infrastructure/
│ └── imdb_client.go
└── config/
└── movie_config.go
