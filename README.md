# Ally Academy:

1. *User Service*:
   - Authentication:
     - POST /api/auth/login: User login.
     - POST /api/auth/logout: User logout.
     - POST /api/auth/register: User registration.
     - POST /api/auth/reset-password: Reset user password.
     - GET /api/auth/user/{user_id}: Listing one user
   - Profile Management:
     - GET /api/profile/{user_id}: Get user profile.
     - PUT /api/profile/update: Update user profile.
     - DELETE /api/profile/delete: Delete user profile.
   - Preferences:
     - GET /api/preferences: Get user preferences.
     - PUT /api/preferences/update: Update user preferences.

2. *Chatbot Service*:
   - Interaction:
     - POST /api/chatbot/ask: Submit a question to the chatbot.
     - POST /api/chatbot/feedback: Provide feedback on chatbot responses.
   - Recommendations:
     - GET /api/recommendations: Get personalized recommendations from the chatbot.

3. *Q&A Service*:
   - Questions:
     - POST /api/questions/ask: Ask a question.
     - GET /api/questions/{question_id}: Get question details.
     - PUT /api/questions/{question_id}/update: Update a question.
     - DELETE /api/questions/{question_id}/delete: Delete a question.
   - Answers:
     - POST /api/questions/{question_id}/answers/post: Post an answer to a question.
     - GET /api/questions/{question_id}/answers: Get answers to a question.
     - PUT /api/questions/{question_id}/answers/{answer_id}/update: Update an answer.
     -POST /api/questions/{question_id}/answers/upvote: Upvote a comment
     - DELETE /api/questions/{question_id}/answers/{answer_id}/delete: Delete an answer.
   - Search:
     - GET /api/questions/search: Search questions by keywords.


4. *Content Service*:
   - Lecture Materials:
     - POST /api/lectures/upload: Upload lecture materials (videos, PDFs, etc.).  (college, subject name in the body)
     - GET /api/lectures/{lecture_id}: Get lecture details.
     - PUT /api/lectures/{lecture_id}/update: Update lecture details.
     - DELETE /api/lectures/{lecture_id}/delete: Delete a lecture.
   - Search:
     - GET /api/lectures/search: Search lecture materials by subject or doctor.

5. *Utility Service*:
   - GPA Calculator:
     - POST /api/gpa/calculate: Calculate GPA.
   - Calendar:
     - POST /api/calendar/event/add: Add an event to the calendar.
     - GET /api/calendar/events: Get calendar events.
     - PUT /api/calendar/event/{event_id}/update: Update a calendar event.
     - DELETE /api/calendar/event/{event_id}/delete: Delete a calendar event.
   - Reminders:
     - POST /api/reminders/add: Add a reminder.
     - GET /api/reminders: Get reminders.
     - PUT /api/reminders/{reminder_id}/update: Update a reminder.
     - DELETE /api/reminders/{reminder_id}/delete: Delete a reminder.

6. *Help Service*:
   - Project Assistance:
     - POST /api/help/request: Request help for a project.
     - GET /api/help/offers: Get offers from other students to help with a project.
     - POST /api/help/payment: Make a payment for project assistance.
   - Peer-to-Peer Interaction:
     - POST /api/help/chat: Initiate a chat with a peer helper.

7. *Admin Service*:
   - User Management:
     - GET /api/admin/users: Get all users.
     - GET /api/admin/users/{user_id}: Get user details.
     - PUT /api/admin/users/{user_id}/update: Update user details.
     - DELETE /api/admin/users/{user_id}/delete: Delete a user.
   - System Management:
     - GET /api/admin/logs: Get system logs.
     - DELETE /api/admin/logs/delete: Delete system logs.