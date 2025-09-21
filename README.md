# Mini School Dashboard API

**Base URL:** [https://mini-school-dashboard-db.vercel.app/](https://mini-school-dashboard-db.vercel.app/)

---

## Students API
- **Endpoint:** `/students.json`  
- **Full URL:** [https://mini-school-dashboard-db.vercel.app/students.json](https://mini-school-dashboard-db.vercel.app/students.json)  
- **Description:** Returns a JSON list of all students.  
- **Example fields:**  
  - `id` → Student ID  
  - `firstName` → First name (smallcase)  
  - `lastName` → Last name (smallcase)  
  - `age` → Age  
  - `grade` → Grade  
  - `class` → Class  

---

## Teachers API
- **Endpoint:** `/teachers.json`  
- **Full URL:** [https://mini-school-dashboard-db.vercel.app/teachers.json](https://mini-school-dashboard-db.vercel.app/teachers.json)  
- **Description:** Returns a JSON list of all teachers.  
- **Example fields:**  
  - `id` → Teacher ID  
  - `firstName` → First name (smallcase)  
  - `lastName` → Last name (smallcase)  
  - `subject` → Subject taught  
  - `email` → Email  
  - `phone` → Phone number  

---

## Example Fetch (JavaScript)
```js
// Fetch students
fetch('https://mini-school-dashboard-db.vercel.app/students.json')
  .then(res => res.json())
  .then(data => console.log(data));

// Fetch teachers
fetch('https://mini-school-dashboard-db.vercel.app/teachers.json')
  .then(res => res.json())
  .then(data => console.log(data));
