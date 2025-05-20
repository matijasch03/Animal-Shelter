# 🐾 Animal Protection Association Application

> Developed as a project for the **Software Specification and Modeling** course at **SIIT**.

This web application simulates the operations of an **animal protection association**, supporting various roles such as administrators, volunteers, members, and guests. The platform facilitates animal care, adoption, donation, and communication.

---

## 📌 Purpose

The app supports a fictional association focused on animal (pet) welfare, enabling efficient communication and task management across different user roles.

---

## 👥 User Roles

- **Admin**
- **Volunteers**
- **Members (Registered Users)**
- **Guests**

---

## 🧑‍💼 Admin Functionalities

- Create the **Association** entity.
- Create the **first volunteer**, who then manages further operations.

---

## 🧑‍🤝‍🧑 Volunteer Functionalities

- Manage animal posts (**Create, Read, Update, Delete**).
- Approve/reject requests to become volunteers (voting system).
- Vote to remove existing volunteers.
- Review and approve/reject post requests from members.
- Rate and comment on members.
- Like and comment on animal posts.
- Import daily bank statements into the app.
- Track which animals have been adopted and by whom.
- Rate experiences with adopters.
- Optionally maintain a **blacklist** of users (e.g., poorly rated).
- Resign from volunteer role.
- Approve new user registration requests.
- Send broadcast messages to all users.
- Block or deactivate users (instead of deletion).
- Soft-delete inappropriate posts (e.g., trolling).

---

## 🐶 Animal Post / Request Attributes

- `type`: e.g., dog, cat
- `breed`: (optional)
- `healthStatus`: healthy, sick, injured, etc.
- `yearOfBirth`: (optional, estimated)
- `isAdopted`: adoption status (can be reversed)
- `media`: images/videos (optional)
- `color`
- `estimatedAge`
- `location`: where the animal was found or is currently
- `authorInfo`: hidden from users
- `status`: `APPROVED` or `REJECTED`

---

## 👤 Member Functionalities

- Submit post requests or edit requests.
- Make anonymous donations (e.g., for veterinary treatment).
- Submit requests for:
  - **Adoption**
  - **Temporary fostering** (select care dates)
- Rate and review animals after fostering (1–5 or comment).
- Rate and comment on animal posts for transparency.
- Request to become a volunteer.
- Send private messages to:
  - Volunteers
  - Anonymous post authors

---

## 🧭 Guest Functionalities

- Browse and search all public animal posts.
- Register (by submitting a request).

---

## 🏢 Association Attributes

- `name`
- `contactInfo`: email, phone number, Instagram
- `address`
- `bankAccount`: 18-digit number for donations (no in-app transactions)
- All **donations and withdrawals** are publicly visible.
- Donation purpose is indicated via payment note (e.g., for a specific animal).
- The app is designed for a **single association**.

---

## ⚙️ Non-Functional Requirements

- Around 20 volunteers and several thousand registered members.
- Moderate usage; no major performance constraints.
- Must operate **24/7**.
- Security: **personal data must be encoded**.

---

## 📂 Notes

This is a conceptual academic project and may not include real payment integration. All data regarding donations and animal statuses are for simulation purposes only.
