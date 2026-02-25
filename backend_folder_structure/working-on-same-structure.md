app/
├── server/
│   └── start.go

booking/
├── constants/
│   └── App_constants
├── controller/
│   ├── booking_controller.go
│   ├── revenue_controller.go
│   ├── shows_controller.go
│   ├── User_controller.go
│   ├── auth_controller.go                 <-- NEW
│   ├── payment_controller.go              <-- NEW
│   ├── seat_controller.go                 <-- NEW
│   ├── checkin_controller.go              <-- NEW
│   ├── notification_controller.go         <-- NEW
│   ├── avatar_controller.go               <-- NEW
│   └── file_upload_controller.go          <-- NEW
├── database/
│   ├── common/
│   │   └── Base_db
│   ├── connection/
│   │   └── connection.go
│   └── seed/
│       └── dataseeder.go
├── dto/
│   ├── request/
│   │   ├── Booking_request
│   │   ├── booking_request_Test
│   │   ├── user_signup_request.go          <-- NEW
│   │   ├── email_verification_request.go   <-- NEW
│   │   ├── phone_verification_request.go   <-- NEW
│   │   ├── login_request.go                <-- NEW
│   │   ├── reset_password_request.go       <-- NEW
│   │   ├── update_user_request.go          <-- NEW
│   │   ├── change_password_request.go      <-- NEW
│   │   ├── captcha_request.go              <-- NEW
│   │   ├── show_schedule_request.go        <-- NEW
│   │   ├── seat_selection_request.go       <-- NEW
│   │   ├── payment_request.go              <-- NEW
│   │   └── checkin_request.go              <-- NEW
│   └── response/
│       ├── Booking_confirmation_response
│       ├── Show_responses
│       ├── user_profile_response.go        <-- NEW
│       ├── auth_response.go                <-- NEW
│       ├── payment_response.go             <-- NEW
│       ├── revenue_dashboard_response.go   <-- NEW
│       ├── seat_map_response.go            <-- NEW
│       ├── imdb_rating_response.go         <-- NEW
│       ├── trailer_response.go             <-- NEW
│       ├── poster_response.go              <-- NEW
│       ├── qr_response.go                  <-- NEW
│       └── csv_download_response.go        <-- NEW
├── Model/
│   ├── booking.go
│   ├── customer.go
│   ├── movie.go
│   ├── show.go
│   ├── slot.go
│   ├── user.go
│   ├── seat.go                           <-- NEW
│   ├── seat_type.go                      <-- NEW
│   ├── screen.go                         <-- NEW
│   ├── payment.go                        <-- NEW
│   ├── transaction.go                    <-- NEW
│   ├── email_verification.go             <-- NEW
│   ├── phone_verification.go             <-- NEW
│   ├── avatar.go                         <-- NEW
│   ├── user_profile_image.go             <-- NEW
│   ├── revenue.go                        <-- NEW
│   ├── checkin.go                        <-- NEW
│   └── qr_ticket.go                      <-- NEW
└── repository/
    ├── booking_Repository
    ├── Customer_repository
    ├── show_repository
    ├── User_repository
    ├── auth_repository.go               <-- NEW
    ├── payment_repository.go            <-- NEW
    ├── seat_repository.go               <-- NEW
    ├── revenue_repository.go            <-- NEW
    ├── checkin_repository.go            <-- NEW
    └── notification_repository.go       <-- NEW

service/
├── Booking_service
├── Revenue_service
├── Shows_service
├── user_Service
├── auth_service.go                     <-- NEW
├── payment_service.go                  <-- NEW
├── seat_service.go                     <-- NEW
├── checkin_service.go                  <-- NEW
├── notification_service.go             <-- NEW
├── captcha_service.go                  <-- NEW
├── imdb_service.go                     <-- NEW
├── file_upload_service.go              <-- NEW
└── qr_service.go                       <-- NEW

common/
└── logger/
    └── logger.go

middleware/
├── cors/
│   └── cors.go
├── security/
│   ├── basic_Auth
│   ├── rbac.go                          <-- NEW
│   ├── jwt_middleware.go                <-- NEW
│   └── rate_limiter.go                  <-- NEW
└── validator/
    ├── Dto_validation_handler
    └── Dto_validator

config/
├── captcha_config.go                   <-- NEW
├── payment_config.go                   <-- NEW
├── email_config.go                     <-- NEW
└── storage_config.go                   <-- NEW

docs/
error/
infrastructure/
├── imdb_client.go                     <-- NEW
├── captcha_client.go                  <-- NEW
├── email_sender.go                    <-- NEW
├── sms_sender.go                      <-- NEW
├── payment_gateway.go                 <-- NEW
├── storage_service.go                 <-- NEW
└── qr_generator.go                    <-- NEW

integration_test/
├── auth_test.go                       <-- NEW
├── booking_test.go                    <-- NEW
├── payment_test.go                    <-- NEW
├── seat_test.go                       <-- NEW
└── revenue_test.go                    <-- NEW

migration/
├── seat_migration.sql                 <-- NEW
├── screen_migration.sql               <-- NEW
├── payment_migration.sql              <-- NEW
├── user_verification_migration.sql    <-- NEW
├── revenue_migration.sql              <-- NEW
└── checkin_migration.sql              <-- NEW

Movieservice/
└── movie_gateway/
    ├── Movie_gateway
    └── Movie_service
```
