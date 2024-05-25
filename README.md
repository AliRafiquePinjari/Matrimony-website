## Procedural Design (Algorithm)

### User Registration Algorithm

**Algorithm Name:** registerUser
**Purpose:** To register a new user with the system.

**Steps:**
1. Begin.
2. Collect user details: name, email, phone, password, dateOfBirth, gender, address.
3. Validate email and phone format.
4. Check if the email or phone already exists in the database.
    - If exists, return error "User already exists."
5. Hash the password for security.
6. Generate a unique UserID.
7. Insert the new user details into the User table.
8. Return success message.
9. End.

### Profile Search Algorithm

**Algorithm Name:** searchProfiles
**Purpose:** To search and return a list of profiles matching the search criteria.

**Steps:**
1. Begin.
2. Receive search criteria (e.g., age range, gender, location, interests).
3. Query the Profile table with the search criteria.
4. Retrieve matching profiles.
5. Return the list of profiles.
6. End.

### Match Acceptance Algorithm

**Algorithm Name:** acceptMatch
**Purpose:** To accept a match between two users.

**Steps:**
1. Begin.
2. Receive userID and matchID.
3. Validate matchID.
4. Update the Match table, setting the status to 'Accepted' for the given matchID.
5. Notify both users of the accepted match.
6. Return success message.
7. End.

### Send Message Algorithm

**Algorithm Name:** sendMessage
**Purpose:** To send a message from one user to another.

**Steps:**
1. Begin.
2. Receive senderID, receiverID, and message content.
3. Validate receiverID.
4. Insert the message into the Message table with the senderID, receiverID, and content.
5. Return success message.
6. End.

### Review Profile Algorithm (Admin Function)

**Algorithm Name:** reviewProfile
**Purpose:** For admin to review and approve or reject a user profile.

**Steps:**
1. Begin.
2. Receive adminID, profileID, status, and comments.
3. Validate adminID and profileID.
4. Update the Profile table, setting the status to the provided status and adding comments.
5. Notify the user of the profile review result.
6. Return success message.
7. End.
