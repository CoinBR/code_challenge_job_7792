
> [!IMPORTANT]  
> Before starting, create a public GitHub/GitLab repository and share the link with the interviewer.

## Code Challenge for Full Stack Engineer (Job 7792)

Build a fullstack app for managing salon appointments. 
This challenge evaluates your proficiency in both frontend and backend development, focusing on GraphQL, PostgreSQL, React, and TypeScript.

 
### Backend 
 
GraphQL API: Implement a GraphQL API that supports the following operations: 
 - [ ] Query: Fetch all appointments with their associated salon and service details
 - [ ] Mutation: Add a new appointment
 - [ ] Mutation: Update an existing appointment's details
 - [ ] Mutation: Delete an appointment
 
PostgreSQL Database: Use PostgreSQL to store the appointment data.
The db should include these tables:
 - [ ] salons with fields: id, name, location.
 - [ ] services with fields: id, salon_id, name, price.
 - [ ] appointments with fields: id, salonId, customerName, serviceName, appointmentTime.
 
Environment: 
   Use any Node.js framework (e.g., Express, Nest) to set up your GraphQL server.
 
### Frontend
 
Develop a simple **React** frontend that interacts with the GraphQL API.


Requirements:
 - [ ] Use **Apollo Client** to interact with the GraphQL API.
 - [ ]  Style the app minimally using plain CSS or a library like TailwindCSS, Material-UI or bootstrap.
 
Features:
 - [ ] View Appointments: Display a list of all appointments fetched from the backend.
 - [ ] Add Appointment: Provide a form to create a new appointment with these fields:
   - Customer Name
   - Salon
   - Service
   - Appointment Time
 
### Constraints 
 
 - [ ] Use clean code practices and adhere to design patterns.
 - [ ] Include a README file with:
   - [ ] Setup instructions.
   - [ ] Brief explanation of your approach.

---

> [!TIP]  
> If you'd like to use this project as a template instead of setting up yours from scratch:

- Create a public GitHub/GitLab repository
- Run this command with your repository URL:
  - `sh export candidate_repo='___YOUR_REPOSITORY_URL___' `
- In the same terminal:
  - Clone this challenge project
  - Navigate to its folder
  - Paste and run the following commands:

```sh
[ "$candidate_repo" = "___YOUR_REPOSITORY_URL___" ] \
  && echo "invalid candidate repo" \
  && exit 1

export original_repo_name='code_challenge_job_7792'
git clone "https://github.com/CoinBR/${original_repo_name}"
cd ${original_repo_name}

rm -rf .git
rm README.md
mv README.md.candidate README.md

git init
git add .
git commit -m "project setup"
git remote add origin ${candidate_repo}
git push -f -u origin master
```

then, to prepare it for your development, run:
- `./run.sh`

