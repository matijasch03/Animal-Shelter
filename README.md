🐾 Animal Protection Association Application
This project is developed as part of the Software Specification and Modeling course at SIIT. It is a web application designed to support the operations of an animal protection association (focused on pets), enabling various roles and interactions around animal care, adoption, and support.

📌 Purpose
The application is intended to simulate the functionality of a fictional animal protection organization, including different user roles and operations related to animal welfare.

👥 User Roles
Admin

Volunteers

Members (Registered Users)

Guests

🧑‍💼 Admin Functionalities
Creates the Association entity.

Creates the first volunteer and delegates all further responsibilities to them and future volunteers.

🧑‍🤝‍🧑 Volunteer Functionalities
Add/edit/delete animal posts (via form).

Vote on membership requests from users who want to become volunteers.

Vote to remove other volunteers (initiated by one, decided by voting).

Review and approve/reject animal post requests submitted by members.

Rate and comment on members.

Like/comment on animal posts.

Import daily bank transaction data into the app (to avoid manual tracking).

View adoption status and history (which user adopted which animal).

Rate the adoption experience with users.

Optionally manage a blacklist of users (e.g., those rated poorly).

Resign from volunteer role (self-remove).

Approve user registration requests.

Send broadcast messages to all users.

Soft-delete inappropriate posts (e.g., trolling).

Block or change status of users instead of deleting them.

🐶 Animal Post / Request Attributes
Type (dog, cat, etc.)

Breed (optional)

Health status (healthy, sick, missing limb, etc.)

Year of birth (not required to be exact)

Adoption status (isAdopted: still shown after adoption, includes possibility of returning the animal)

Media: photos/videos (optional)

Color

Estimated age

Location (found or currently staying)

Author Info: hidden from regular users

Request Status: APPROVED / REJECTED

👤 Member Functionalities
Send requests for new posts or editing existing posts.

Make anonymous donations (e.g., for treatment at a veterinary clinic).

Submit requests for:

Adoption

Temporary care (select available dates)

Rate animals they’ve cared for (1–5 or comment).

Comment and rate animal posts to help future adopters.

Request to become a volunteer.

Send private messages to:

Volunteers

Anonymous post authors

🧭 Guest Functionalities
View and search animal posts.

Submit registration request.

🏢 Association Attributes
Name

Contact info: email, phone, Instagram

Address

Bank account number (18 digits, used for donations — no in-app payments)

All donations and expenses are publicly visible.

Donation purpose is specified (e.g., animal name) using the payment message field.

Application supports a single association.

⚙️ Non-Functional Requirements
Expected user base: ~20 volunteers, several thousand registered members.

Moderate traffic; not performance-critical.

Application must run reliably 24/7.

Security: encoding of personal data is required.
