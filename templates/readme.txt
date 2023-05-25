## Step 1 - Project Setup & Flask Basics


- Create a project on GitHub 
- Open up the project on Replit
- Create and run a Flask web server
- Push changes back to GitHub



SQL Statement to Create jobs Table

CREATE TABLE jobs (
  id INT NOT NULL AUTO_INCREMENT,
  title VARCHAR(120) NOT NULL,
  location VARCHAR(120) NOT NULL,
  salary INT,
  currency VARCHAR(10),
  responsibilities VARCHAR(2000),
  requirements VARCHAR(2000),
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
  PRIMARY KEY (id)
);

SQL Statement to Create applications Table

CREATE TABLE applications (
  id INT NOT NULL AUTO_INCREMENT,
  job_id INT NOT NULL,
  full_name VARCHAR(250) NOT NULL,
  email VARCHAR(250) NOT NULL,
  linkedin_url VARCHAR(500),
  education VARCHAR(2000),
  work_experience VARCHAR(2000),
  resume_url VARCHAR(500),
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
  PRIMARY KEY (id)
);

